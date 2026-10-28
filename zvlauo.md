代发 wailian999

readonly PI=3.14
来源：http://hz.zhiwuduotai.top/gteejusypi.html

[R04] 位置参数
来源：http://hz.316326.xyz/gtmnmusebq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zycfv.cn/gtornmjfxd.html

[R05] 参数默认值
来源：http://hz.yj20258888.top/gtqivsiced.html

name="${1:-default}"
来源：http://hz.yonumen.top/gthyjfaphj.html

[R06] 判断命令是否存在
来源：http://hz.shanyushiyangkeji.top/gtqxwizqrz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zdqjudy.top/gtgohqmpbk.html

[R07] if 判断文件
来源：http://hz.meibo888.top/gtmziezhdp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhiwuduotai.top/gtotksojcr.html

[R08] 数值比较
来源：http://hz.hnxiangtu.top/gtfecxzhgh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cheryme.top/gtxeyjwqer.html

[R09] 字符串比较
来源：http://hz.yj202588.top/gtdbeuorog.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xylfe.cn/gtzcbogyyl.html

[R10] 正则匹配
来源：http://hz.cdnleiting.top/gtctmijmwq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgfzy.top/gtdyyycpxz.html

[R11] case 多分支
来源：http://hz.mhx1999.top/gtmwflzbsd.html

case "$1" in
来源：http://hz.hfpthk.cn/gtjwswzpfe.html

start) echo "启动" ;;
来源：http://hz.meibo888.top/gtazizscwy.html

stop)  echo "停止" ;;
来源：http://hz.hnxiangtu.top/gtvbnsemkd.html

*)     echo "未知命令" ;;
来源：http://hz.shuidangran.top/gtvvfmloer.html

esac
来源：http://hz.jqgfzy.top/gtufgkqrie.html

[R12] for 遍历文件
来源：http://hz.zhoulong.xyz/gtkyqxgwqb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.mhx1999.top/gtyspchixu.html

[R13] for 计数循环
来源：http://hz.yangfankeji.com/gtuqqoqrme.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tian-w.cn/gtpsrcjuft.html

[R14] C 风格 for
来源：http://hz.gzhubu.top/gthdzycvhl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinyuanbaomall.cn/gtenjgtrii.html

[R15] while 逐行读文件
来源：http://hz.pycfn.com/gtmryorbxw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.52xcode.cn/gtxqfvlbzl.html

[R16] until 等待条件
来源：http://hz.quarkkingdee.top/gtxowhhooy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sweek.top/gtpkysldmr.html

[R17] 数组定义与取值
来源：http://hz.cdnleiting.top/gtwluctblz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gotoacloud.top/gtflujpesj.html

[R18] 遍历数组
来源：http://hz.xuetiantiany.cn/gtuxbrszuf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yuxming.cn/gtsefhstvj.html

[R19] 数组长度
来源：http://hz.ybcxt.top/gtlgiuhfzv.html

echo "${#arr[@]}"
来源：http://hz.smart0.xyz/gtrmxtrfke.html

[R20] 关联数组（字典）
来源：http://hz.bjfxy.top/gtfxvpbkij.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinqigufen.top/gtukmtysuc.html

[R21] 字符串长度
来源：http://hz.yuanzhike.top/gtgkhovzuz.html

echo "${#s}"
来源：http://hz.hfpthk.cn/gtnexggeoo.html

[R22] 截取子串
来源：http://hz.yueranfly.top/gtwekbuhty.html

echo "${s:0:5}"
来源：http://hz.tian-w.cn/gtmdleyrfv.html

[R23] 字符串替换
来源：http://hz.9152youxi.cn/gtwbcnoxhm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.316326.xyz/gtlhqidrvm.html

[R24] 大小写转换
来源：http://hz.gogol.net.cn/gtyoroyvfw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj202588.top/gtgorgkuws.html

[R25] 去后缀 / 去前缀
来源：http://hz.feifeiyinyue.top/gtreeqybky.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.mhx1999.top/gtuwqtunkh.html

[R26] 命令替换
来源：http://hz.yangfankeji.com/gtyeugpbib.html

now=$(date +%F); echo "$now"
来源：http://hz.hongshengwenyu.top/gtwqpzqcxr.html

[R27] 算术展开
来源：http://hz.hongshengwenyu.top/gtgiqycbbc.html

echo $((1 + 2 * 3))
来源：http://hz.shanyushiyangkeji.top/gthxvkpngh.html

[R28] 浮点运算
来源：http://hz.smart0.xyz/gtirfzmnlu.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhoulong.xyz/gtlfcfusul.html

[R29] 定义函数
来源：http://hz.sysykeji.top/gtlggjmhuj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.redwolf501.top/gtscwvttnl.html

[R30] 函数返回状态码
来源：http://hz.hnxiangtu.top/gtttafmoto.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhaomingkeji.xyz/gtpoaeoxxw.html

[R31] 局部变量
来源：http://hz.smart0.xyz/gtypyoensq.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenzaomai.com/gtiajdnuax.html

[R32] 参数个数校验
来源：http://hz.xylfe.cn/gtuoscafog.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hongshengwenyu.top/gtwppleviw.html

[R33] 捕获错误并提示行号
来源：http://hz.nanxuanxn.top/gtvqwlwkpd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.andypj.xyz/gtzbmohhzh.html

[R34] 退出时清理
来源：http://hz.chenjidiqi.icu/gtyegpongo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gtyqedqxyw.html

[R35] 后台执行并等待
来源：http://hz.andypj.xyz/gtxajcgfvy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xingfuxueyuan.xyz/gtrfvwnzky.html

[R36] 并发执行多个任务
来源：http://hz.quarkkingdee.top/gtwfomeuqh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.smart0.xyz/gtnwsydnch.html

[R37] 把输出赋给变量
来源：http://hz.hammf.cn/gtjhvigmcq.html

files=$(ls -1)
来源：http://hz.hammf.cn/gtehpjybpq.html

[R38] 管道串联
来源：http://hz.jianghu66.top/gtelqsexal.html

cat a.txt | grep -i error | wc -l
来源：http://hz.pycfn.com/gtbwbcxkjs.html

[R39] 重定向标准输出与错误
来源：http://hz.bjfxy.top/gtcilohrsh.html

cmd > out.log 2>&1
来源：http://hz.vqdsnc.cn/gtbbkedxfe.html

[R40] 追加写日志
来源：http://hz.mhx1999.top/gtkqokyviv.html

echo "log" >> out.log
来源：http://hz.gzhubu.top/gtdcnwlnop.html

[R41] 丢弃输出
来源：http://hz.316326.xyz/gtcxwxxewc.html

cmd >/dev/null 2>&1
来源：http://hz.yongpay.top/gtdrrisdkt.html

[R42] 输入重定向
来源：http://hz.jqgufenzy.top/gtovmrkaoh.html

wc -l < a.txt
来源：http://hz.9152youxi.cn/gtvalkfvsu.html

[R43] 按名字查找文件
来源：http://hz.hammf.cn/gtencnrsmf.html

find . -name "*.log" -type f
来源：http://hz.fengsongda.top/gtnsuereif.html

[R44] 按修改时间查找
来源：http://hz.yj20258.top/gtzjdvacte.html

find . -mtime -7 -type f
来源：http://hz.ybcxt.top/gtbrbgzgbg.html

[R45] 批量删除
来源：http://hz.yvedp.cn/gthqfthzla.html

find . -name "*.tmp" -delete
来源：http://hz.tanke756.top/gtmtygpbwn.html

[R46] 递归替换文件内容
来源：http://hz.52xcode.cn/gtkrjwpafo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sxryk.cn/gtxsxtubjj.html

[R47] sed 单行替换
来源：http://hz.zhengqikj.top/gtmqaqnxxo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.pengpengdd.cyou/gtitspakld.html

[R48] awk 取指定列
来源：http://hz.jinyuanbaomall.cn/gttyvmxclk.html

awk '{print $1, $3}' a.txt
来源：http://hz.shuidangran.top/gtcsptrqzq.html

[R49] awk 带条件
来源：http://hz.ybcxt.top/gtomkepqvz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zycfv.cn/gtwmhthvao.html

[R50] awk 求和
来源：http://hz.guannengcc.top/gtwulfiejx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sxryk.cn/gtevhuddkm.html

[R51] 排序去重取前几
来源：http://hz.jinqigfzy.top/gtgqimvmtp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.wangshuangyany.cn/gtezlxhtbw.html

[R52] 统计行数
来源：http://hz.hywenlv.cn/gtdexikyvg.html

wc -l a.txt
来源：http://hz.gogol.net.cn/gtmymvtcgt.html

[R53] 查看文件头与实时尾
来源：http://hz.yj20258888.top/gtgbugbdvw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ybcxt.top/gtwgyhrhin.html

[R54] 比较两个文件
来源：http://hz.yueranfly.top/gtbfmsrgys.html

diff a.txt b.txt
来源：http://hz.zhoulong.xyz/gtebxlnqnd.html

[R55] 压缩与解压
来源：http://hz.cucudq.cn/gtpkafeqlp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.0kj1m.cn/gteicpornc.html

[R56] 远程拷贝
来源：http://hz.chenjidiqi.icu/gtnfhpyoff.html

scp file user@host:/path/
来源：http://hz.cucudq.cn/gtilyhohbv.html

[R57] 远程执行命令
来源：http://hz.chenjidiqi.icu/gtjcslifzy.html

ssh user@host 'uptime'
来源：http://hz.daria6918.cn/gthusxunrs.html

[R58] 下载文件
来源：http://hz.jinqigfzy.top/gtrklytoil.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.daxiang520.top/gtqvofhcyp.html

[R59] 发 POST JSON
来源：http://hz.wangdashe.top/gtbnspiqbm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.meibo888.top/gtiwuxzorg.html

[R60] 只看 HTTP 状态码
来源：http://hz.redwolf501.top/gtdgxkvvpi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinqigufen.top/gtsnynfchb.html

[R61] 磁盘占用
来源：http://hz.zhaomingkeji.xyz/gtktyzwrzr.html

df -h;  du -sh *
来源：http://hz.xylfe.cn/gtatxzfipr.html

[R62] 找最占空间的文件
来源：http://hz.aibaodan.cn/gtfkughval.html

du -ah . | sort -rh | head -10
来源：http://hz.vqdsnc.cn/gtghumuehu.html

[R63] 内存与进程
来源：http://hz.yongpay.top/gtinuauxlb.html

free -h;  ps aux | grep nginx
来源：http://hz.zhongyouzk.top/gtkxbdsuku.html

[R64] 结束进程
来源：http://hz.wangshuangyany.cn/gtcgzazkjd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.feifeiyinyue.top/gttxgmvpzl.html

[R65] 查看端口占用
来源：http://hz.chenlongwang.top/gtqvamenui.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cucudq.cn/gtymngungb.html

[R66] 定时任务
来源：http://hz.tianlin.xyz/gtvgbwmjxa.html

crontab -e;  crontab -l
来源：http://hz.fzhhl.top/gtqbuoancj.html

[R67] 生成随机十六进制串
来源：http://hz.aizwys.cn/gtajdtsltk.html

openssl rand -hex 16
来源：http://hz.shuidangran.top/gtrhmqukuv.html

[R68] 计算文件校验值
来源：http://hz.smart0.xyz/gtgclrkdju.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.bjfxy.top/gtmkvskkcp.html

[R69] 生成随机密码
来源：http://hz.pycfn.com/gtisadhbnz.html

head -c 16 /dev/urandom | base64
来源：http://hz.xuetiantiany.cn/gtqyrojdfn.html

[R70] 时间戳与互转
来源：http://hz.chenjidiqi.icu/gtcsxynzge.html

date +%s;  date -d @1700000000
来源：http://hz.ydzc1.top/gtejiyrkqc.html

[R71] 日期格式化
来源：http://hz.gaohongyu789.top/gtcdsetzit.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ehwqpu.com/gtmcxmfzyu.html

[R72] 等待端口就绪
来源：http://hz.yj20258888.top/gtabemekvu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sweek.top/gtemtiqute.html

[R73] 分割大日志
来源：http://hz.yongpay.top/gtvjwinado.html

split -l 1000 big.log part_
来源：http://hz.shzxlz.cn/gtlnttneqq.html

[R74] 批量重命名
来源：http://hz.jiagoushi.top/gtcwdhqyma.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.andypj.xyz/gtypwjyrxb.html

[R75] 导出环境变量
来源：http://hz.sweek.top/gtwmetelld.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nanxinkj.top/gthqrrrhmt.html

[R76] 使用临时文件
来源：http://hz.sweek.top/gtgthzwoij.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zdqjudy.top/gtkwcztfxz.html

[R77] 读取用户输入
来源：http://hz.snrcjt.cn/gttpdijhdy.html

read -rp "请输入: " ans
来源：http://hz.daxiang520.top/gthbyzjhoz.html

[R78] 交互式菜单
来源：http://hz.sweek.top/gtcxwnkvsu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jqgfzy.top/gtzrhnijxo.html

[R79] 解析命令行选项
来源：http://hz.jyoumei.cn/gtancgeuyo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cashguo.top/gtfpkmouag.html

[R80] 查看脚本执行耗时
来源：http://hz.wangdashe.top/gtypatpsdx.html

time ./run.sh
来源：http://hz.mhx1999.top/gtzltkcgtp.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtftjekxmm.html

S. C / C++ 专题
来源：http://hz.xziqi.cn/gtbedwjqjt.html

================================================================================
来源：http://hz.hammf.cn/gtjouksrzk.html

[S01] C：Hello World
来源：http://hz.cdnleiting.top/gtifltgguw.html

#include <stdio.h>
来源：http://hz.hongshengwenyu.top/gtmynulihp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.meibo888.top/gtsdiytauf.html

[S02] C：变量与格式化输出
来源：http://hz.shzxlz.cn/gtfhfnlwiu.html

int a = 10; printf("%d\n", a);
来源：http://hz.316326.xyz/gtgjvppnnj.html

[S03] C：读入整数
来源：http://hz.zhijiandao.cn/gtivjykezu.html

int x; scanf("%d", &x);
来源：http://hz.yj202588.top/gtilvmthhr.html

[S04] C：字符串复制
来源：http://hz.aizwys.cn/gtzdtkzxhb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tian-w.cn/gttdftdifq.html

[S05] C：字符串长度
来源：http://hz.meibo888.top/gtqgyrcvzi.html

strlen(s)
来源：http://hz.ywan-chungtsiang.top/gtgcbyywkp.html

[S06] C：字符串比较
来源：http://hz.pengpengdd.cyou/gtdxdeupqq.html

strcmp(a, b) == 0
来源：http://hz.birdmap.top/gtccwoldjn.html

[S07] C：数组遍历求和
来源：http://hz.yangfankeji.com/gtkuxushbd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.redwolf501.top/gtlrutzkuy.html

[S08] C：动态内存分配与释放
来源：http://hz.52xcode.cn/gtkcykdstw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jiagoushi.top/gtqorfvjeg.html

[S09] C：结构体定义与初始化
来源：http://hz.bjfxy.top/gtzhccoegh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhaomingkeji.xyz/gtyyginxkc.html

[S10] C：指针与解引用
来源：http://hz.yj202588.top/gtwrtopgpq.html

int *p = &a;  *p = 5;
来源：http://hz.sweek.top/gtmbmtbhqn.html

[S11] C：逐行读文件
来源：http://hz.xylfe.cn/gthmdqnlfo.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ydzc1.top/gtgystonyl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.aibaodan.cn/gtcpngwdpz.html

fclose(f);
来源：http://hz.snrcjt.cn/gtzxllfuoc.html

[S12] C：写文件
来源：http://hz.iojbl.cn/gtsmtgxgwb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.wangshuangyany.cn/gtikbmirjx.html

[S13] C：宏定义
来源：http://hz.jinqigufen.top/gtwohoaxdd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinghuilouyu.cn/gtulzoegwy.html

[S14] C：枚举
来源：http://hz.meibo888.top/gtfajrqcoj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.chenjidiqi.icu/gtfubtduvh.html

[S15] C：类型转换
来源：http://hz.jianghu66.top/gteaqazkio.html

(double) a / b
来源：http://hz.daxiang520.top/gtfryqpxfo.html

[S16] C：位操作置位
来源：http://hz.jyoumei.cn/gtjnnxiops.html

x |= (1 << 3);
来源：http://hz.yuxming.cn/gttyiykwew.html

[S17] C：安全拼接字符串
来源：http://hz.sweek.top/gttzjcenra.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.redwolf501.top/gtytscfplc.html

[S18] C：命令行参数
来源：http://hz.dianchejie.cn/gtalxvgaeh.html

int main(int argc, char **argv)
来源：http://hz.feifeiyinyue.top/gtdrfynwic.html

[S19] C：快速排序
来源：http://hz.birdmap.top/gtlomctsrx.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.guannengcc.top/gtgvyjorgg.html

[S20] C：二分查找
来源：http://hz.yvedp.cn/gtfubymdws.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gaohongyu789.top/gtsbarwvbj.html

[S21] C：字符类别判断
来源：http://hz.sxryk.cn/gtfzrchoek.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgufenzy.top/gtjcfytvru.html

[S22] C：字符串转数字
来源：http://hz.jianghu66.top/gtkkrajqni.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.vqdsnc.cn/gtsbholito.html

[S23] C：随机数
来源：http://hz.quarkkingdee.top/gtmnkwvfgx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daria6918.cn/gtjnxyowhf.html

[S24] C：获取本地时间
来源：http://hz.jinyuanbaomall.cn/gtdsqdseqy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinqigufen.top/gtdfyydghd.html

[S25] C：内存拷贝
来源：http://hz.quarkkingdee.top/gtnzofpulz.html

memcpy(dst, src, n);
来源：http://hz.nanxuanxn.top/gttpfmnrzx.html

[S26] C：内存清零
来源：http://hz.mhx1999.top/gtecskjxvp.html

memset(a, 0, sizeof a);
来源：http://hz.xuetiantiany.cn/gtykncwobl.html

[S27] C：定义常量
来源：http://hz.jlsjyb.cn/gtsshbkzvp.html

const double PI = 3.14159;
来源：http://hz.zhongyouzk.top/gtffptlazv.html

[S28] C：静态变量
来源：http://hz.snrcjt.cn/gtwdmdujyx.html

static int counter = 0;
来源：http://hz.snrcjt.cn/gtmjukentj.html

[S29] C：变参函数
来源：http://hz.sxryk.cn/gtyruzodca.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ivvv.top/gtkhritdwd.html

[S30] C：头文件保护
来源：http://hz.svipenyu.cn/gtnbguhdrw.html

#ifndef X_H
来源：http://hz.meibo888.top/gtjkppwgeh.html

#define X_H
来源：http://hz.yj202588.top/gtcnceurug.html

#endif
来源：http://hz.zhoulong.xyz/gtnhepatnh.html

[S31] C++：Hello World
来源：http://hz.tianlin.xyz/gtplrxwyty.html

#include <iostream>
来源：http://hz.cucudq.cn/gtwwodxrmi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jianghu66.top/gtxrahlxce.html

[S32] C++：字符串
来源：http://hz.gotoacloud.top/gtoiuhsujr.html

std::string s = "hi";  s += "!";
来源：http://hz.jinghuilouyu.cn/gtebkecywq.html

[S33] C++：vector 增删
来源：http://hz.ydjk.org.cn/gtbvthhsjs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuanzhike.top/gtlfuccpvu.html

[S34] C++：遍历 vector
来源：http://hz.zdqjudy.top/gtezddvnow.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.redwolf501.top/gtbgrzmjsq.html

[S35] C++：map
来源：http://hz.daria6918.cn/gteztnuadh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pycfn.com/gtwinszwfd.html

[S36] C++：unordered_map
来源：http://hz.hysaishi.cn/gtxgpquimo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zycfv.cn/gtapnfkycf.html

[S37] C++：set
来源：http://hz.ydjk.org.cn/gtaantzljy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shzxlz.cn/gtrniijygv.html

[S38] C++：排序
来源：http://hz.dashuyun.cn/gtqxenuozk.html

std::sort(v.begin(), v.end());
来源：http://hz.zhaomingkeji.xyz/gtysucztoc.html

[S39] C++：自定义比较器排序
来源：http://hz.mhx1999.top/gtgwylepsx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.c1oappe.top/gthnzvhgak.html

[S40] C++：查找元素
来源：http://hz.zdqjudy.top/gtproqtrgc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gzhubu.top/gttmyqltaj.html

[S41] C++：类与构造函数
来源：http://hz.gotoacloud.top/gttjjdsjlq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shanyushiyangtech.top/gtlerbyiaw.html

[S42] C++：继承与虚函数
来源：http://hz.mhx1999.top/gtovvprszd.html

class B : public Base { public: void f() override {} };
来源：http://hz.shanyushiyangtech.top/gtchhnjcvq.html

[S43] C++：智能指针
来源：http://hz.hongshengwenyu.top/gtxmfabidu.html

auto p = std::make_unique<int>(5);
来源：http://hz.yonumen.top/gtjfsuwokc.html

[S44] C++：引用传参
来源：http://hz.vqdsnc.cn/gtvveqyfmv.html

void inc(int &x) { ++x; }
来源：http://hz.ywan-chungtsiang.top/gtrbqyjswj.html

[S45] C++：lambda
来源：http://hz.zhengqikj.top/gtrdvtobig.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yvedp.cn/gtidwopivr.html

[S46] C++：函数模板
来源：http://hz.wangdashe.top/gtrqcttolj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gotoacloud.top/gtbmxfegfn.html

[S47] C++：结构化绑定遍历
来源：http://hz.xingfuxueyuan.xyz/gttjhmhkch.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhoulong.xyz/gtdjsiaubh.html

[S48] C++：逐行读文件
来源：http://hz.cdnleiting.top/gtftrsvzqh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.dashuyun.cn/gtinmnvzlj.html

while (std::getline(in, line)) { }
来源：http://hz.hongshengwenyu.top/gtvxfalciw.html

[S49] C++：写文件
来源：http://hz.feifeiyinyue.top/gtwhhgdtvh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nwbrower.top/gtefhorhmt.html

[S50] C++：格式化数字
来源：http://hz.jqgfzy.top/gtrhxqkvfx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.pengpengdd.cyou/gtgxfxyyut.html

[S51] C++：显式类型转换
来源：http://hz.yueranfly.top/gtmltyaqaz.html

static_cast<double>(a) / b
来源：http://hz.xinyue.icu/gtwxphacpu.html

[S52] C++：const 与 noexcept
来源：http://hz.ppjwa.cn/gtgdzwxypm.html

int size() const noexcept { return n_; }
来源：http://hz.yvedp.cn/gtampbtaoy.html

[S53] C++：移动语义
来源：http://hz.tanke756.top/gtgrupzlra.html

std::vector<int> w = std::move(v);
来源：http://hz.gogol.net.cn/gtweaztcrt.html

[S54] C++：异常处理
来源：http://hz.pycfn.com/gtqigcrsct.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.fzhhl.top/gtricinzjv.html

[S55] C++：结构化绑定
来源：http://hz.hammf.cn/gtulgsnynb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ppjwa.cn/gtlaymsavg.html

[S56] C++：optional
来源：http://hz.chenjidiqi.icu/gtnfktavxm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.daxiang520.top/gteeepgbzb.html

[S57] C++：编译期常量
来源：http://hz.hfpthk.cn/gtjuxdlrob.html

constexpr int N = 10;
来源：http://hz.shuidangran.top/gtygnwmbex.html

[S58] C++：命名空间
来源：http://hz.hywenlv.cn/gtxzdasiis.html

namespace ns { int f() { return 1; } }
来源：http://hz.iojbl.cn/gtsxlzpsqi.html

[S59] C++：静态断言
来源：http://hz.wangshuangyany.cn/gtyfwtuhbq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.dashuyun.cn/gttglpzucy.html

[S60] C++：遍历并删除元素
来源：http://hz.jyoumei.cn/gtmygdminz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangtech.top/gtepuwrvjm.html

================================================================================
来源：http://hz.gotoacloud.top/gtcleejpum.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ybcxt.top/gtmkwmbveg.html

================================================================================
来源：http://hz.hfpthk.cn/gteiksacsg.html

[T01] Kotlin：Hello World
来源：http://hz.hnxiangtu.top/gtdwllzspk.html

println("Hello")
来源：http://hz.ydzc1.top/gteffyuzsq.html

[T02] Kotlin：变量
来源：http://hz.sysykeji.top/gtqbahgxib.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jlsjyb.cn/gtchfkkzuz.html

[T03] Kotlin：字符串模板
来源：http://hz.gogol.net.cn/gtpjsfjils.html

"值: $b"
来源：http://hz.dianchejie.cn/gtllrgxfru.html

[T04] Kotlin：空安全
来源：http://hz.zhongyouzk.top/gtciocaavw.html

val n: String? = null;  n?.length
来源：http://hz.zhengqikj.top/gtnwwocmjq.html


<!-- 参考信息 -->