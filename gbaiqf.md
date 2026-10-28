代发 wailian999

set -euo pipefail
来源：http://hz.jinghuilouyu.cn/gtbnceeamw.html

[R02] 变量赋值与使用
来源：http://hz.tian-w.cn/gtgttnbxvr.html

name="Tom"; echo "$name"
来源：http://hz.pengpengdd.cyou/gtzwzznxci.html

[R03] 只读变量
来源：http://hz.xingfuxueyuan.xyz/gtylbpwcwz.html

readonly PI=3.14
来源：http://hz.fengsongda.top/gtoouivjto.html

[R04] 位置参数
来源：http://hz.cheryme.top/gtqiiynrot.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.tanke756.top/gtxcrxvkcn.html

[R05] 参数默认值
来源：http://hz.zhongyouzk.top/gtcgidrksu.html

name="${1:-default}"
来源：http://hz.smart0.xyz/gtddskqkvs.html

[R06] 判断命令是否存在
来源：http://hz.iojbl.cn/gtsicbwtfu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hysaishi.cn/gtafewatug.html

[R07] if 判断文件
来源：http://hz.xylfe.cn/gtslbxxibl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinqigufen.top/gtkjkodwnk.html

[R08] 数值比较
来源：http://hz.c1oappe.top/gtlqsirrar.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.52xcode.cn/gtpejjuuoc.html

[R09] 字符串比较
来源：http://hz.cucudq.cn/gtsjiltcku.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhiwuduotai.top/gtbzvnzqgv.html

[R10] 正则匹配
来源：http://hz.daxiang520.top/gtnhunbebo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sufxvd.cn/gtckalxwpg.html

[R11] case 多分支
来源：http://hz.aibaodan.cn/gtcvdeobof.html

case "$1" in
来源：http://hz.xylfe.cn/gtdkqkouoo.html

start) echo "启动" ;;
来源：http://hz.pycfn.com/gtiqsclqwi.html

stop)  echo "停止" ;;
来源：http://hz.daria6918.cn/gtatffcobs.html

*)     echo "未知命令" ;;
来源：http://hz.nwbrower.top/gthfqeqdmb.html

esac
来源：http://hz.nwbrower.top/gtpudxuldj.html

[R12] for 遍历文件
来源：http://hz.jinqigfzy.top/gtqdjygztx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.nanxinkj.top/gtawlgfoqy.html

[R13] for 计数循环
来源：http://hz.bjfxy.top/gtthlnalrp.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.pycfn.com/gtrnrmrrrl.html

[R14] C 风格 for
来源：http://hz.shangyingyoupin.top/gtussiavan.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.aibaodan.cn/gtlvprobvz.html

[R15] while 逐行读文件
来源：http://hz.guannengcc.top/gtmgjrphxi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daria6918.cn/gtjhkceipe.html

[R16] until 等待条件
来源：http://hz.chenjidiqi.icu/gtjccaapks.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yangfankeji.com/gtysquusfr.html

[R17] 数组定义与取值
来源：http://hz.meibo888.top/gtluevjawn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shangyingyoupin.top/gtoldmvvtu.html

[R18] 遍历数组
来源：http://hz.nanxinkj.top/gtczbtccco.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yj202588.top/gtrwrvqavp.html

[R19] 数组长度
来源：http://hz.jianghu66.top/gtvmiihxku.html

echo "${#arr[@]}"
来源：http://hz.hongshengwenyu.top/gtvxrshnbh.html

[R20] 关联数组（字典）
来源：http://hz.wangdashe.top/gtonllryyc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.wangshuangyany.cn/gtsadtzyyd.html

[R21] 字符串长度
来源：http://hz.fengsongda.top/gtxlvkxayl.html

echo "${#s}"
来源：http://hz.redwolf501.top/gtkwmxlrkg.html

[R22] 截取子串
来源：http://hz.vqdsnc.cn/gtudvkgpxx.html

echo "${s:0:5}"
来源：http://hz.bjfxy.top/gtzrjctbva.html

[R23] 字符串替换
来源：http://hz.wangshuangyany.cn/gtaumkoqio.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sysykeji.top/gtzslnswdq.html

[R24] 大小写转换
来源：http://hz.svipenyu.cn/gtluwfxbgi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cdnleiting.top/gtpdbzshbj.html

[R25] 去后缀 / 去前缀
来源：http://hz.zycfv.cn/gtyygelezj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.guowangkeji.top/gtzzpbnkkn.html

[R26] 命令替换
来源：http://hz.meibo888.top/gtapekoldb.html

now=$(date +%F); echo "$now"
来源：http://hz.vqdsnc.cn/gtlmhearsg.html

[R27] 算术展开
来源：http://hz.jlsjyb.cn/gtsgzuyerb.html

echo $((1 + 2 * 3))
来源：http://hz.quarkkingdee.top/gtfgobeoej.html

[R28] 浮点运算
来源：http://hz.smart0.xyz/gtaacshwht.html

echo "scale=2; 10/3" | bc
来源：http://hz.havefunace.top/gthzqetiea.html

[R29] 定义函数
来源：http://hz.xziqi.cn/gtyzyiohgs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shanyushiyangtech.top/gtaijgylyf.html

[R30] 函数返回状态码
来源：http://hz.smart0.xyz/gtfkaoagzg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.meibo888.top/gtqxpxjuzn.html

[R31] 局部变量
来源：http://hz.smart0.xyz/gtnrlsumgp.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhaomingkeji.xyz/gtlbzgzelk.html

[R32] 参数个数校验
来源：http://hz.316326.xyz/gtkepvsnff.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jianghu66.top/gtpuekisnc.html

[R33] 捕获错误并提示行号
来源：http://hz.sxryk.cn/gtzubgnehv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.aizwys.cn/gtfojqbipe.html

[R34] 退出时清理
来源：http://hz.aibaodan.cn/gtmaktvwze.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangkeji.top/gtkdglqttp.html

[R35] 后台执行并等待
来源：http://hz.dashuyun.cn/gtmbmzmmif.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.birdmap.top/gtriivvran.html

[R36] 并发执行多个任务
来源：http://hz.jinqigufen.top/gtuckjwzkl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.0kj1m.cn/gtnhrtvtjg.html

[R37] 把输出赋给变量
来源：http://hz.wangdashe.top/gthkhshdkl.html

files=$(ls -1)
来源：http://hz.pengpengdd.cyou/gtpfmjshyn.html

[R38] 管道串联
来源：http://hz.zhoulong.xyz/gtsgyzeegm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tianlin.xyz/gtqehfduuc.html

[R39] 重定向标准输出与错误
来源：http://hz.jqgfzy.top/gtcwehfkin.html

cmd > out.log 2>&1
来源：http://hz.jqgfzy.top/gthnhcxvrt.html

[R40] 追加写日志
来源：http://hz.nanxuanxn.top/gthuqnhlog.html

echo "log" >> out.log
来源：http://hz.cucudq.cn/gtwwdbzrje.html

[R41] 丢弃输出
来源：http://hz.jinyuanbaomall.cn/gtnjbuwscu.html

cmd >/dev/null 2>&1
来源：http://hz.zhongyouzk.top/gtnfffbkud.html

[R42] 输入重定向
来源：http://hz.mhx1999.top/gtrhaoztqc.html

wc -l < a.txt
来源：http://hz.wangshuangyany.cn/gtslohramd.html

[R43] 按名字查找文件
来源：http://hz.jinqigufen.top/gtvvdbhkrp.html

find . -name "*.log" -type f
来源：http://hz.zhengqikj.top/gtblmrqpow.html

[R44] 按修改时间查找
来源：http://hz.yangfankeji.com/gtlttpvjyk.html

find . -mtime -7 -type f
来源：http://hz.ehwqpu.com/gtkvgxelsa.html

[R45] 批量删除
来源：http://hz.jyoumei.cn/gtivjpasvl.html

find . -name "*.tmp" -delete
来源：http://hz.meibo888.top/gtrlpphisl.html

[R46] 递归替换文件内容
来源：http://hz.xylfe.cn/gttjmudjho.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinghuilouyu.cn/gtygnamzdq.html

[R47] sed 单行替换
来源：http://hz.hysaishi.cn/gtcymlbvwh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jqgfzy.top/gthmnfyvnk.html

[R48] awk 取指定列
来源：http://hz.fzhhl.top/gtqupvfitm.html

awk '{print $1, $3}' a.txt
来源：http://hz.mhx1999.top/gtiahjlcil.html

[R49] awk 带条件
来源：http://hz.quarkkingdee.top/gtmqmwvalh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hongshengwenyu.top/gtmxsjqopd.html

[R50] awk 求和
来源：http://hz.jlsjyb.cn/gtlvwnrdpe.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jianghu66.top/gtcszbjzcx.html

[R51] 排序去重取前几
来源：http://hz.sysykeji.top/gtuezbpjqt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ybcxt.top/gtujcdnayx.html

[R52] 统计行数
来源：http://hz.redwolf501.top/gtbbmhdbvj.html

wc -l a.txt
来源：http://hz.daxiang520.top/gtjmccsdnb.html

[R53] 查看文件头与实时尾
来源：http://hz.aibaodan.cn/gtgzkjspvw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ehwqpu.com/gtwwdnzkya.html

[R54] 比较两个文件
来源：http://hz.52xcode.cn/gtkewtdghn.html

diff a.txt b.txt
来源：http://hz.cdnleiting.top/gtbixpdngk.html

[R55] 压缩与解压
来源：http://hz.jinqigufen.top/gtgcazgiza.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhaomingkeji.xyz/gtmduqczlc.html

[R56] 远程拷贝
来源：http://hz.yongpay.top/gtuoohhemc.html

scp file user@host:/path/
来源：http://hz.zycfv.cn/gtdrjydlxa.html

[R57] 远程执行命令
来源：http://hz.yanxiufei.cn/gtzkhdmtjz.html

ssh user@host 'uptime'
来源：http://hz.gotoacloud.top/gtzztrlzmf.html

[R58] 下载文件
来源：http://hz.hongshengwenyu.top/gtqleuoqrk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ywan-chungtsiang.top/gtynuokqdy.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangtech.top/gtztpjcamg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jlsjyb.cn/gtideulhrr.html

[R60] 只看 HTTP 状态码
来源：http://hz.ehwqpu.com/gtrcevnlia.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yonumen.top/gtyfclhnsh.html

[R61] 磁盘占用
来源：http://hz.yangfankeji.com/gthohsaswo.html

df -h;  du -sh *
来源：http://hz.cheryme.top/gtfkbcpscf.html

[R62] 找最占空间的文件
来源：http://hz.zhiwuduotai.top/gtixxpwrbs.html

du -ah . | sort -rh | head -10
来源：http://hz.tian-w.cn/gtnjeghbdx.html

[R63] 内存与进程
来源：http://hz.kuanghao11.cn/gtpfwzqikb.html

free -h;  ps aux | grep nginx
来源：http://hz.havefunace.top/gtqkxzmgvj.html

[R64] 结束进程
来源：http://hz.iojbl.cn/gtptmkrkal.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhiwuduotai.top/gtfwvyoaou.html

[R65] 查看端口占用
来源：http://hz.havefunace.top/gtopramwbd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuanzhike.top/gtklrqqkgj.html

[R66] 定时任务
来源：http://hz.yuanzhike.top/gtpufasjji.html

crontab -e;  crontab -l
来源：http://hz.jqgufenzy.top/gtilyrdtww.html

[R67] 生成随机十六进制串
来源：http://hz.feifeiyinyue.top/gthmivhivq.html

openssl rand -hex 16
来源：http://hz.snrcjt.cn/gtkeaaujhh.html

[R68] 计算文件校验值
来源：http://hz.vqdsnc.cn/gtkfzuzgyn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xziqi.cn/gtdpzcreaj.html

[R69] 生成随机密码
来源：http://hz.guannengcc.top/gtlisppdpc.html

head -c 16 /dev/urandom | base64
来源：http://hz.zdqjudy.top/gtamzeontq.html

[R70] 时间戳与互转
来源：http://hz.shuidangran.top/gtsvkgvhvd.html

date +%s;  date -d @1700000000
来源：http://hz.smart0.xyz/gtexhfnmjj.html

[R71] 日期格式化
来源：http://hz.yuxming.cn/gtavfravjk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.haohaochexian.top/gttjwgoutu.html

[R72] 等待端口就绪
来源：http://hz.jinghuilouyu.cn/gtpyoclbbr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.c1oappe.top/gtohhfvevl.html

[R73] 分割大日志
来源：http://hz.svipenyu.cn/gtkrsqemnr.html

split -l 1000 big.log part_
来源：http://hz.dianchejie.cn/gtgligxqpa.html

[R74] 批量重命名
来源：http://hz.sysykeji.top/gtchvlilwz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhaomingkeji.xyz/gtqdvzkqsp.html

[R75] 导出环境变量
来源：http://hz.snrcjt.cn/gtzdxqmtme.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shangyingyoupin.top/gtzffgomgv.html

[R76] 使用临时文件
来源：http://hz.zhaomingkeji.xyz/gtigdxeezb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhengqikj.top/gtanclxddi.html

[R77] 读取用户输入
来源：http://hz.andypj.xyz/gtimmqnkvs.html

read -rp "请输入: " ans
来源：http://hz.feifeiyinyue.top/gtmlndxutv.html

[R78] 交互式菜单
来源：http://hz.pycfn.com/gtwntrwlyz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.dianchejie.cn/gtwkiphfpd.html

[R79] 解析命令行选项
来源：http://hz.cheryme.top/gtneidepww.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.birdmap.top/gthfixbvqj.html

[R80] 查看脚本执行耗时
来源：http://hz.xinyue.icu/gtcoithdww.html

time ./run.sh
来源：http://hz.hfpthk.cn/gthmrmujte.html

================================================================================
来源：http://hz.sxryk.cn/gttofyycvk.html

S. C / C++ 专题
来源：http://hz.haohaochexian.top/gtcfvrebdj.html

================================================================================
来源：http://hz.pycfn.com/gttitticfe.html

[S01] C：Hello World
来源：http://hz.jqgfzy.top/gtymzsokwu.html

#include <stdio.h>
来源：http://hz.sufxvd.cn/gttwjanunh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yvedp.cn/gtswuyvukw.html

[S02] C：变量与格式化输出
来源：http://hz.ydzc1.top/gtyocrbunh.html

int a = 10; printf("%d\n", a);
来源：http://hz.yvedp.cn/gtupcgudmn.html

[S03] C：读入整数
来源：http://hz.zdqjudy.top/gttzztlqvy.html

int x; scanf("%d", &x);
来源：http://hz.chenzaomai.com/gtmgabjtrc.html

[S04] C：字符串复制
来源：http://hz.ybcxt.top/gtazxoexlj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinghuilouyu.cn/gtoglwjisi.html

[S05] C：字符串长度
来源：http://hz.9152youxi.cn/gtdzlqxqey.html

strlen(s)
来源：http://hz.xinyue.icu/gtrcnrhrqz.html

[S06] C：字符串比较
来源：http://hz.ywan-chungtsiang.top/gtxghyzzgz.html

strcmp(a, b) == 0
来源：http://hz.shuidangran.top/gtkijejxsc.html

[S07] C：数组遍历求和
来源：http://hz.xuanzx.com/gtzvwarqks.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhijiandao.cn/gtejhnillz.html

[S08] C：动态内存分配与释放
来源：http://hz.jianghu66.top/gtdgizphpd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ywan-chungtsiang.top/gtsnxnqnzi.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxuanxn.top/gtcobnyztw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinghuilouyu.cn/gttskunovr.html

[S10] C：指针与解引用
来源：http://hz.yonumen.top/gtfhubggsu.html

int *p = &a;  *p = 5;
来源：http://hz.yonumen.top/gtksrisbzb.html

[S11] C：逐行读文件
来源：http://hz.dashuyun.cn/gtrtqbcfgf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.smart0.xyz/gtdcxjzyul.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yangfankeji.com/gtehodniyr.html

fclose(f);
来源：http://hz.zhixingplan.top/gtcumudbwi.html

[S12] C：写文件
来源：http://hz.cashguo.top/gtupchjong.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.andypj.xyz/gtsqprleeu.html

[S13] C：宏定义
来源：http://hz.tian-w.cn/gtfaedvdin.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hongshengwenyu.top/gtbomtftpa.html

[S14] C：枚举
来源：http://hz.hnqzz.top/gtdmkdsjlk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xylfe.cn/gtpljotqaq.html

[S15] C：类型转换
来源：http://hz.gotoacloud.top/gtestpgnoa.html

(double) a / b
来源：http://hz.jiagoushi.top/gtmtkwphhm.html

[S16] C：位操作置位
来源：http://hz.yongpay.top/gtezbmtfum.html

x |= (1 << 3);
来源：http://hz.fzhhl.top/gtcdrnxkbv.html

[S17] C：安全拼接字符串
来源：http://hz.jinqigfzy.top/gtuuioasnh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sufxvd.cn/gtwkwbecmu.html

[S18] C：命令行参数
来源：http://hz.zhaomingkeji.xyz/gtxscywjvq.html

int main(int argc, char **argv)
来源：http://hz.zhongyouzk.top/gtshvmorig.html

[S19] C：快速排序
来源：http://hz.hnqzz.top/gterybvqnr.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hnqzz.top/gtskzqgiin.html

[S20] C：二分查找
来源：http://hz.xziqi.cn/gtxfkujtob.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtpxyykvrs.html

[S21] C：字符类别判断
来源：http://hz.tanke756.top/gtcraqexqm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.fengsongda.top/gtfkabxysv.html

[S22] C：字符串转数字
来源：http://hz.tanke756.top/gtsokktqoh.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guowangkeji.top/gtwefzxvpm.html

[S23] C：随机数
来源：http://hz.nanxinkj.top/gtpqckbtlk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.havefunace.top/gtspwuiwoo.html

[S24] C：获取本地时间
来源：http://hz.pycfn.com/gtfoblyjya.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cheryme.top/gtslqbbytg.html

[S25] C：内存拷贝
来源：http://hz.shanyushiyangtech.top/gtkintftjv.html

memcpy(dst, src, n);
来源：http://hz.0kj1m.cn/gthflgrzvp.html

[S26] C：内存清零
来源：http://hz.shzxlz.cn/gtfgzgfldg.html

memset(a, 0, sizeof a);
来源：http://hz.chenlongwang.top/gtkmarodnl.html

[S27] C：定义常量
来源：http://hz.yuxming.cn/gtrsqfyxza.html

const double PI = 3.14159;
来源：http://hz.hysaishi.cn/gtjapgjhah.html

[S28] C：静态变量
来源：http://hz.ehwqpu.com/gtyrhanltu.html

static int counter = 0;
来源：http://hz.hnqzz.top/gtjbllhole.html

[S29] C：变参函数
来源：http://hz.pycfn.com/gtnkwhhldj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hammf.cn/gtmnivwugd.html

[S30] C：头文件保护
来源：http://hz.xziqi.cn/gtikqwpavo.html

#ifndef X_H
来源：http://hz.shanyushiyangkeji.top/gtxecdkrjp.html

#define X_H
来源：http://hz.dianchejie.cn/gtfhywerlv.html

#endif
来源：http://hz.ehwqpu.com/gtsbfedldp.html

[S31] C++：Hello World
来源：http://hz.tian-w.cn/gtgekneqzc.html

#include <iostream>
来源：http://hz.yj20258.top/gtrbbywzsb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daxiang520.top/gtjxogkrwk.html

[S32] C++：字符串
来源：http://hz.kuanghao11.cn/gtnzboarbx.html

std::string s = "hi";  s += "!";
来源：http://hz.fengsongda.top/gtxmscbxll.html

[S33] C++：vector 增删
来源：http://hz.zhaomingkeji.xyz/gtkclysjxi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xziqi.cn/gtwaawumkh.html

[S34] C++：遍历 vector
来源：http://hz.wangdashe.top/gtldigvewv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hnqzz.top/gteppzmham.html

[S35] C++：map
来源：http://hz.xuetiantiany.cn/gtijvnedhm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhijiandao.cn/gtrexcwcnv.html

[S36] C++：unordered_map
来源：http://hz.hammf.cn/gtonlkpfvn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.feifeiyinyue.top/gtevfpiuap.html

[S37] C++：set
来源：http://hz.dianchejie.cn/gtxszpurxh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jiagoushi.top/gttwlyijpc.html

[S38] C++：排序
来源：http://hz.zhixingplan.top/gtbiywndif.html

std::sort(v.begin(), v.end());
来源：http://hz.ywan-chungtsiang.top/gtyquooirm.html

[S39] C++：自定义比较器排序
来源：http://hz.snrcjt.cn/gtfoshqvwz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.andypj.xyz/gtmofqxzfw.html

[S40] C++：查找元素
来源：http://hz.xylfe.cn/gtrzjhmupj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.daxiang520.top/gtsokwvrmf.html

[S41] C++：类与构造函数
来源：http://hz.wangdashe.top/gtqcywtaxu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinghuilouyu.cn/gtbkxfxgvy.html

[S42] C++：继承与虚函数
来源：http://hz.zhoulong.xyz/gtorhuhity.html

class B : public Base { public: void f() override {} };
来源：http://hz.hfpthk.cn/gtqjqqjahh.html

[S43] C++：智能指针
来源：http://hz.ehwqpu.com/gtcoxjgdbh.html

auto p = std::make_unique<int>(5);
来源：http://hz.cucudq.cn/gtagxvnzpa.html

[S44] C++：引用传参
来源：http://hz.bjfxy.top/gtvkkmqqfu.html

void inc(int &x) { ++x; }
来源：http://hz.cdnleiting.top/gtuggyvtei.html

[S45] C++：lambda
来源：http://hz.ivvv.top/gtgkzoztzx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.chenlongwang.top/gtwxcdpeyg.html

[S46] C++：函数模板
来源：http://hz.haohaochexian.top/gtnanyjltr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinqigfzy.top/gtlpjtxctx.html

[S47] C++：结构化绑定遍历
来源：http://hz.ydzc1.top/gttquvvvnr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.52xcode.cn/gtyqmnmgkp.html

[S48] C++：逐行读文件
来源：http://hz.xinyue.icu/gtyscsdpdb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.smart0.xyz/gtdsodxgjq.html

while (std::getline(in, line)) { }
来源：http://hz.shanyushiyangkeji.top/gthkbdqjlb.html

[S49] C++：写文件
来源：http://hz.zycfv.cn/gtnjlrlgmc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hysaishi.cn/gtqhgxkvas.html

[S50] C++：格式化数字
来源：http://hz.gogol.net.cn/gthynbagma.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jyoumei.cn/gtfjdvgwmi.html

[S51] C++：显式类型转换
来源：http://hz.dianchejie.cn/gtvzqaizgm.html

static_cast<double>(a) / b
来源：http://hz.ybcxt.top/gtqdqblkhn.html

[S52] C++：const 与 noexcept
来源：http://hz.pycfn.com/gtgxbozgpl.html

int size() const noexcept { return n_; }
来源：http://hz.316326.xyz/gtucbhmspf.html

[S53] C++：移动语义
来源：http://hz.nanxuanxn.top/gtmgglrsbo.html

std::vector<int> w = std::move(v);
来源：http://hz.daria6918.cn/gtfvwaqrmn.html

[S54] C++：异常处理
来源：http://hz.zhixingplan.top/gtjjxbapsw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.redwolf501.top/gthrjbrcjv.html

[S55] C++：结构化绑定
来源：http://hz.jqgufenzy.top/gtqfvvdkkz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.guannengcc.top/gtqchvsbdn.html

[S56] C++：optional
来源：http://hz.yvedp.cn/gtiuezhfqv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yj20258.top/gtpmvddnzh.html

[S57] C++：编译期常量
来源：http://hz.zhoulong.xyz/gtinbbvyyt.html

constexpr int N = 10;
来源：http://hz.zhixingplan.top/gtrnqmltjs.html

[S58] C++：命名空间
来源：http://hz.cqqwz.cn/gtzzbqwbxm.html

namespace ns { int f() { return 1; } }
来源：http://hz.chenjidiqi.icu/gtsjvdjfbn.html

[S59] C++：静态断言
来源：http://hz.yangfankeji.com/gtpjzctmoj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.birdmap.top/gtrthfcdie.html

[S60] C++：遍历并删除元素
来源：http://hz.ydzc1.top/gtkliykeaz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuxming.cn/gtaqrrojph.html

================================================================================
来源：http://hz.gotoacloud.top/gtdbpoevbd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhoulong.xyz/gtejfhqqvm.html

================================================================================
来源：http://hz.shuidangran.top/gtgvwklngm.html

[T01] Kotlin：Hello World
来源：http://hz.0kj1m.cn/gtqhgosbys.html

println("Hello")
来源：http://hz.bjfxy.top/gtxpydjydr.html

[T02] Kotlin：变量
来源：http://hz.zycfv.cn/gtvlzexcug.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gogol.net.cn/gtqjwwxkwm.html


<!-- 参考信息 -->