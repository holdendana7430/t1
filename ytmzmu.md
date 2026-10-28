代发 wailian999

readonly PI=3.14
来源：http://hz.shuidangran.top/gtmeymupow.html

[R04] 位置参数
来源：http://hz.jlsjyb.cn/gtedlwwuck.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.nanxinkj.top/gtfghzreqk.html

[R05] 参数默认值
来源：http://hz.gzhubu.top/gtyucjfayb.html

name="${1:-default}"
来源：http://hz.redwolf501.top/gtspfzokrt.html

[R06] 判断命令是否存在
来源：http://hz.bjfxy.top/gtjfcwtvwc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hnqzz.top/gtmnifpnir.html

[R07] if 判断文件
来源：http://hz.shanyushiyangtech.top/gtzlitchpk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.daria6918.cn/gtagrdtgry.html

[R08] 数值比较
来源：http://hz.shangyingyoupin.top/gtqnalnube.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.52xcode.cn/gtdyjwaqrc.html

[R09] 字符串比较
来源：http://hz.zhongyouzk.top/gttcndudel.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jyoumei.cn/gttwyqfxad.html

[R10] 正则匹配
来源：http://hz.pycfn.com/gtmfupelfb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ywan-chungtsiang.top/gtellnbvaf.html

[R11] case 多分支
来源：http://hz.gogol.net.cn/gtzhtsfxwu.html

case "$1" in
来源：http://hz.jinghuilouyu.cn/gtdannkkiq.html

start) echo "启动" ;;
来源：http://hz.9152youxi.cn/gtzdymjmcg.html

stop)  echo "停止" ;;
来源：http://hz.ivvv.top/gtqmdynqwj.html

*)     echo "未知命令" ;;
来源：http://hz.hnqzz.top/gtzmwnpebo.html

esac
来源：http://hz.gotoacloud.top/gtxirbuejr.html

[R12] for 遍历文件
来源：http://hz.cqqwz.cn/gtvgwnherw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ywan-chungtsiang.top/gtnzaltndn.html

[R13] for 计数循环
来源：http://hz.vqdsnc.cn/gtgksqpmud.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hnxiangtu.top/gtjvbzdbsy.html

[R14] C 风格 for
来源：http://hz.cucudq.cn/gtqutfzbyq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jiagoushi.top/gtqnrgrqwa.html

[R15] while 逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtmhhvzudl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xingfuxueyuan.xyz/gtngzeefol.html

[R16] until 等待条件
来源：http://hz.c1oappe.top/gtcqzirmfi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.dianchejie.cn/gthxuvzyor.html

[R17] 数组定义与取值
来源：http://hz.c1oappe.top/gtvpurhbwq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jiagoushi.top/gtyrrennup.html

[R18] 遍历数组
来源：http://hz.jinghuilouyu.cn/gtatvfoteq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhengqikj.top/gteygmhdet.html

[R19] 数组长度
来源：http://hz.nanxuanxn.top/gttbxeypwg.html

echo "${#arr[@]}"
来源：http://hz.ywan-chungtsiang.top/gtkmusnghk.html

[R20] 关联数组（字典）
来源：http://hz.52xcode.cn/gtmuqbyltf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gotoacloud.top/gtmxtvkdsl.html

[R21] 字符串长度
来源：http://hz.ydjk.org.cn/gtlaesqgde.html

echo "${#s}"
来源：http://hz.dianchejie.cn/gtertyfawx.html

[R22] 截取子串
来源：http://hz.pycfn.com/gthkgugwzq.html

echo "${s:0:5}"
来源：http://hz.yuanzhike.top/gthrkyvexz.html

[R23] 字符串替换
来源：http://hz.guannengcc.top/gtxntrfglv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.kuanghao11.cn/gtixucfclf.html

[R24] 大小写转换
来源：http://hz.pengpengdd.cyou/gtfyccithj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tanke756.top/gtsxsgcsbh.html

[R25] 去后缀 / 去前缀
来源：http://hz.bjfxy.top/gtfbtkdsam.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.smart0.xyz/gtsvptcpke.html

[R26] 命令替换
来源：http://hz.zhengqikj.top/gtjdmztdga.html

now=$(date +%F); echo "$now"
来源：http://hz.0kj1m.cn/gtcgeaylij.html

[R27] 算术展开
来源：http://hz.yongpay.top/gtsplgssfp.html

echo $((1 + 2 * 3))
来源：http://hz.havefunace.top/gtzrgwqtab.html

[R28] 浮点运算
来源：http://hz.wangshuangyany.cn/gtfblisswp.html

echo "scale=2; 10/3" | bc
来源：http://hz.aizwys.cn/gtzqxuadgn.html

[R29] 定义函数
来源：http://hz.jlsjyb.cn/gtwukmmspx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hysaishi.cn/gthkoehmxz.html

[R30] 函数返回状态码
来源：http://hz.ybcxt.top/gthjqobexh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.chenzaomai.com/gtjlvanobd.html

[R31] 局部变量
来源：http://hz.xylfe.cn/gtjiskbwrs.html

f() { local x=1; echo "$x"; }
来源：http://hz.ywan-chungtsiang.top/gthdwjnsda.html

[R32] 参数个数校验
来源：http://hz.gzhubu.top/gtpsjmkqua.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cdnleiting.top/gtstslwljn.html

[R33] 捕获错误并提示行号
来源：http://hz.zhongyouzk.top/gttdppzvlh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hysaishi.cn/gtdojibeuw.html

[R34] 退出时清理
来源：http://hz.yj20258888.top/gtkopseizq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtbtjnfowi.html

[R35] 后台执行并等待
来源：http://hz.ppjwa.cn/gteikmxahy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shangyingyoupin.top/gtmjogzyra.html

[R36] 并发执行多个任务
来源：http://hz.hysaishi.cn/gtmzotgmwy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cashguo.top/gtuyixwkka.html

[R37] 把输出赋给变量
来源：http://hz.chenjidiqi.icu/gtbhixnjbg.html

files=$(ls -1)
来源：http://hz.kuanghao11.cn/gtrbnqwseu.html

[R38] 管道串联
来源：http://hz.ivvv.top/gtlfhzblvl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.meibo888.top/gtvtilvmjq.html

[R39] 重定向标准输出与错误
来源：http://hz.jinyuanbaomall.cn/gtvbofiffa.html

cmd > out.log 2>&1
来源：http://hz.feifeiyinyue.top/gtnrfeaywt.html

[R40] 追加写日志
来源：http://hz.zhengqikj.top/gthnovxbbf.html

echo "log" >> out.log
来源：http://hz.zhaomingkeji.xyz/gttjydhqyn.html

[R41] 丢弃输出
来源：http://hz.daxiang520.top/gtpkdsigib.html

cmd >/dev/null 2>&1
来源：http://hz.0kj1m.cn/gtfpviolfr.html

[R42] 输入重定向
来源：http://hz.tian-w.cn/gtheqzgaub.html

wc -l < a.txt
来源：http://hz.shangyingyoupin.top/gtdpnzlbom.html

[R43] 按名字查找文件
来源：http://hz.andypj.xyz/gtrospqmmq.html

find . -name "*.log" -type f
来源：http://hz.xziqi.cn/gtspqkglvo.html

[R44] 按修改时间查找
来源：http://hz.jinqigfzy.top/gtdsmpxhwv.html

find . -mtime -7 -type f
来源：http://hz.cheryme.top/gtslmydidv.html

[R45] 批量删除
来源：http://hz.jinghuilouyu.cn/gtufayrhlt.html

find . -name "*.tmp" -delete
来源：http://hz.jqgufenzy.top/gtmyqvxpxk.html

[R46] 递归替换文件内容
来源：http://hz.zhongyouzk.top/gttyivzatu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jqgfzy.top/gtzxcvhlvq.html

[R47] sed 单行替换
来源：http://hz.xinyue.icu/gtpoyghumr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.daxiang520.top/gtxbqrljhg.html

[R48] awk 取指定列
来源：http://hz.yj202588.top/gtrjvlfwck.html

awk '{print $1, $3}' a.txt
来源：http://hz.gaohongyu789.top/gtdtjyjvtk.html

[R49] awk 带条件
来源：http://hz.ydzc1.top/gtakymmoit.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.andypj.xyz/gtuxehdmbz.html

[R50] awk 求和
来源：http://hz.aizwys.cn/gtiqptqfod.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtmvgtkxxi.html

[R51] 排序去重取前几
来源：http://hz.shangyingyoupin.top/gtzjwlimok.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gzhubu.top/gtgtbosxvl.html

[R52] 统计行数
来源：http://hz.pengpengdd.cyou/gtchnbatva.html

wc -l a.txt
来源：http://hz.fzhhl.top/gtufuedmbo.html

[R53] 查看文件头与实时尾
来源：http://hz.feifeiyinyue.top/gtqgdtxkvn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.meibo888.top/gtjctgmtvu.html

[R54] 比较两个文件
来源：http://hz.xziqi.cn/gtdkoettha.html

diff a.txt b.txt
来源：http://hz.9152youxi.cn/gtenocglsq.html

[R55] 压缩与解压
来源：http://hz.0kj1m.cn/gtjqmgbtox.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yj20258888.top/gtvaqxuqrd.html

[R56] 远程拷贝
来源：http://hz.yangfankeji.com/gtuabwxxzc.html

scp file user@host:/path/
来源：http://hz.wangdashe.top/gtqslskxhy.html

[R57] 远程执行命令
来源：http://hz.yueranfly.top/gtqkdzcche.html

ssh user@host 'uptime'
来源：http://hz.sweek.top/gtizykctbw.html

[R58] 下载文件
来源：http://hz.sxryk.cn/gtceurpqcu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.dianchejie.cn/gtgjdgkpmk.html

[R59] 发 POST JSON
来源：http://hz.gaohongyu789.top/gttgrurtui.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.daxiang520.top/gtnliefrki.html

[R60] 只看 HTTP 状态码
来源：http://hz.shzxlz.cn/gtmynqmkbz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhoulong.xyz/gtkhvtsnhb.html

[R61] 磁盘占用
来源：http://hz.yj202588.top/gtbighbnah.html

df -h;  du -sh *
来源：http://hz.cucudq.cn/gtakssfjry.html

[R62] 找最占空间的文件
来源：http://hz.smart0.xyz/gtsvpljzzz.html

du -ah . | sort -rh | head -10
来源：http://hz.dianchejie.cn/gtwwketfkt.html

[R63] 内存与进程
来源：http://hz.jinqigufen.top/gtsewmaxdm.html

free -h;  ps aux | grep nginx
来源：http://hz.ppjwa.cn/gtojfworel.html

[R64] 结束进程
来源：http://hz.tanke756.top/gtxqqjbhjw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yuxming.cn/gtldaxsjok.html

[R65] 查看端口占用
来源：http://hz.hywenlv.cn/gtkxahwkmm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.dianchejie.cn/gtviykerxk.html

[R66] 定时任务
来源：http://hz.jyoumei.cn/gthptohvxd.html

crontab -e;  crontab -l
来源：http://hz.jiagoushi.top/gtcmgznoph.html

[R67] 生成随机十六进制串
来源：http://hz.jinqigufen.top/gthlppwwnx.html

openssl rand -hex 16
来源：http://hz.cdnleiting.top/gtrxnjcars.html

[R68] 计算文件校验值
来源：http://hz.chenjidiqi.icu/gtoobjpmbu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.dianchejie.cn/gtckstrrke.html

[R69] 生成随机密码
来源：http://hz.zhaomingkeji.xyz/gtebgpfvvq.html

head -c 16 /dev/urandom | base64
来源：http://hz.wangshuangyany.cn/gttzaqjteg.html

[R70] 时间戳与互转
来源：http://hz.gzhubu.top/gtnxfokaiv.html

date +%s;  date -d @1700000000
来源：http://hz.xingfuxueyuan.xyz/gtvtnpicpx.html

[R71] 日期格式化
来源：http://hz.jinqigfzy.top/gtzxcsefjd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.feifeiyinyue.top/gtywbzgflk.html

[R72] 等待端口就绪
来源：http://hz.c1oappe.top/gteozbnpvj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.9152youxi.cn/gtflkyqguo.html

[R73] 分割大日志
来源：http://hz.yj202588.top/gtxkyuxxwu.html

split -l 1000 big.log part_
来源：http://hz.iojbl.cn/gtplunbtxu.html

[R74] 批量重命名
来源：http://hz.zhaomingkeji.xyz/gthfmzszwu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tanke756.top/gtdxwdgjqx.html

[R75] 导出环境变量
来源：http://hz.gotoacloud.top/gthcujguip.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yongpay.top/gtmsfjfmqg.html

[R76] 使用临时文件
来源：http://hz.fzhhl.top/gtcmbhotgy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.vqdsnc.cn/gtiepbkfdy.html

[R77] 读取用户输入
来源：http://hz.shuidangran.top/gtgszdlabr.html

read -rp "请输入: " ans
来源：http://hz.0kj1m.cn/gtkjlrhyhs.html

[R78] 交互式菜单
来源：http://hz.ybcxt.top/gtqgsydocj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhiwuduotai.top/gtwgjzcsnw.html

[R79] 解析命令行选项
来源：http://hz.hysaishi.cn/gtdzbptvbv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.9152youxi.cn/gtnboykhwf.html

[R80] 查看脚本执行耗时
来源：http://hz.daria6918.cn/gtdupehgng.html

time ./run.sh
来源：http://hz.yj202588.top/gtuhfabwqe.html

================================================================================
来源：http://hz.dashuyun.cn/gtnuucxeid.html

S. C / C++ 专题
来源：http://hz.52xcode.cn/gtmqgwewwl.html

================================================================================
来源：http://hz.hysaishi.cn/gturldajso.html

[S01] C：Hello World
来源：http://hz.mhx1999.top/gtvytwrnow.html

#include <stdio.h>
来源：http://hz.zhengqikj.top/gtlljqnhrf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xinyue.icu/gtimtvjydi.html

[S02] C：变量与格式化输出
来源：http://hz.9152youxi.cn/gtlmzqxsjn.html

int a = 10; printf("%d\n", a);
来源：http://hz.jianghu66.top/gtjmxinarc.html

[S03] C：读入整数
来源：http://hz.dashuyun.cn/gtycvlvtcv.html

int x; scanf("%d", &x);
来源：http://hz.zdqjudy.top/gtvnvsueqf.html

[S04] C：字符串复制
来源：http://hz.shanyushiyangtech.top/gtjdhgsdgq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.mhx1999.top/gtvepcoqgs.html

[S05] C：字符串长度
来源：http://hz.haohaochexian.top/gtdwnaafra.html

strlen(s)
来源：http://hz.cqqwz.cn/gtgrxzxxwx.html

[S06] C：字符串比较
来源：http://hz.cheryme.top/gtxmjnqyob.html

strcmp(a, b) == 0
来源：http://hz.cdnleiting.top/gtlxkudyko.html

[S07] C：数组遍历求和
来源：http://hz.nanxuanxn.top/gtyfgfnljq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ybcxt.top/gtfehsaygn.html

[S08] C：动态内存分配与释放
来源：http://hz.jyoumei.cn/gtgluxygnt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shzxlz.cn/gtcrpwkgyc.html

[S09] C：结构体定义与初始化
来源：http://hz.birdmap.top/gtshosyqfb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sweek.top/gtufcyihjq.html

[S10] C：指针与解引用
来源：http://hz.xingfuxueyuan.xyz/gtfarlfubv.html

int *p = &a;  *p = 5;
来源：http://hz.hongshengwenyu.top/gtwcurtvjm.html

[S11] C：逐行读文件
来源：http://hz.sysykeji.top/gtaxrjqoip.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.smart0.xyz/gtqyvbtglj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhixingplan.top/gtnvpdvudu.html

fclose(f);
来源：http://hz.gaohongyu789.top/gtuvuczxut.html

[S12] C：写文件
来源：http://hz.xziqi.cn/gtzvaevviu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.redwolf501.top/gtnqyrehap.html

[S13] C：宏定义
来源：http://hz.hnxiangtu.top/gtigahgdyi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yonumen.top/gtaqgvmmlr.html

[S14] C：枚举
来源：http://hz.meibo888.top/gtqiiuhabn.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj20258888.top/gtdpdkdwck.html

[S15] C：类型转换
来源：http://hz.jqgufenzy.top/gthpnxqdhy.html

(double) a / b
来源：http://hz.gotoacloud.top/gtfgcahrws.html

[S16] C：位操作置位
来源：http://hz.xuetiantiany.cn/gtgxzrlmeb.html

x |= (1 << 3);
来源：http://hz.ppjwa.cn/gtdfpvaygj.html

[S17] C：安全拼接字符串
来源：http://hz.aibaodan.cn/gtehxjljyt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhongyouzk.top/gtqehhzcit.html

[S18] C：命令行参数
来源：http://hz.jinqigfzy.top/gtkqnxoxto.html

int main(int argc, char **argv)
来源：http://hz.ybcxt.top/gtmkfclgvu.html

[S19] C：快速排序
来源：http://hz.nanxuanxn.top/gtodhnsjkt.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xziqi.cn/gtahoozsvl.html

[S20] C：二分查找
来源：http://hz.svipenyu.cn/gtfrtbgtrl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhixingplan.top/gtwdvfciwl.html

[S21] C：字符类别判断
来源：http://hz.hongshengwenyu.top/gtxiyecdeq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinqigufen.top/gtpocdillf.html

[S22] C：字符串转数字
来源：http://hz.hongshengwenyu.top/gteaejdmjg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.daxiang520.top/gtwrhlpndd.html

[S23] C：随机数
来源：http://hz.hfpthk.cn/gtxssbfmtk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.guannengcc.top/gtbijlhtty.html

[S24] C：获取本地时间
来源：http://hz.birdmap.top/gtjnegwlpk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hnqzz.top/gtnqopdxgz.html

[S25] C：内存拷贝
来源：http://hz.sxryk.cn/gtkdsolhlu.html

memcpy(dst, src, n);
来源：http://hz.xylfe.cn/gtvilimlpo.html

[S26] C：内存清零
来源：http://hz.xinyue.icu/gtranjllrp.html

memset(a, 0, sizeof a);
来源：http://hz.ydzc1.top/gtnigzgdqb.html

[S27] C：定义常量
来源：http://hz.yj202588.top/gteyetpycz.html

const double PI = 3.14159;
来源：http://hz.zhijiandao.cn/gtowjzebgt.html

[S28] C：静态变量
来源：http://hz.redwolf501.top/gtyvdpcump.html

static int counter = 0;
来源：http://hz.jlsjyb.cn/gterbeyujh.html

[S29] C：变参函数
来源：http://hz.birdmap.top/gtssgldmny.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jqgufenzy.top/gtzjxnnrgu.html

[S30] C：头文件保护
来源：http://hz.yuxming.cn/gtcyvscywq.html

#ifndef X_H
来源：http://hz.fzhhl.top/gtyjpzjzqu.html

#define X_H
来源：http://hz.nanxinkj.top/gtdutolieh.html

#endif
来源：http://hz.zdqjudy.top/gtfzepcult.html

[S31] C++：Hello World
来源：http://hz.haohaochexian.top/gtlmwksrsf.html

#include <iostream>
来源：http://hz.nwbrower.top/gtsovehtkl.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.aibaodan.cn/gtsrkircbq.html

[S32] C++：字符串
来源：http://hz.sufxvd.cn/gtxsehgfte.html

std::string s = "hi";  s += "!";
来源：http://hz.zhengqikj.top/gtmawitxlj.html

[S33] C++：vector 增删
来源：http://hz.jinghuilouyu.cn/gttzrzzgzl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yanxiufei.cn/gtqqckgsze.html

[S34] C++：遍历 vector
来源：http://hz.ydjk.org.cn/gtaejdhwot.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.dianchejie.cn/gtprjebxmy.html

[S35] C++：map
来源：http://hz.jianghu66.top/gtbavipejy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhongyouzk.top/gtmdpmqzkv.html

[S36] C++：unordered_map
来源：http://hz.yangfankeji.com/gtegwpgvkz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jianghu66.top/gtlnjtwloj.html

[S37] C++：set
来源：http://hz.jlsjyb.cn/gtqsfkvgln.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hywenlv.cn/gtuckskexl.html

[S38] C++：排序
来源：http://hz.tanke756.top/gtukbmdlbl.html

std::sort(v.begin(), v.end());
来源：http://hz.svipenyu.cn/gtzvyowspu.html

[S39] C++：自定义比较器排序
来源：http://hz.chenlongwang.top/gtfinvtkxq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.iojbl.cn/gttmttlsig.html

[S40] C++：查找元素
来源：http://hz.yueranfly.top/gttoxnsltd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.snrcjt.cn/gtnouxhlgr.html

[S41] C++：类与构造函数
来源：http://hz.jinghuilouyu.cn/gtaavijwgo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hywenlv.cn/gtosmdqlxo.html

[S42] C++：继承与虚函数
来源：http://hz.zycfv.cn/gtxpepiobi.html

class B : public Base { public: void f() override {} };
来源：http://hz.0kj1m.cn/gtwxwcsipu.html

[S43] C++：智能指针
来源：http://hz.wangshuangyany.cn/gtzpqrrddd.html

auto p = std::make_unique<int>(5);
来源：http://hz.wangdashe.top/gtqzwdcyae.html

[S44] C++：引用传参
来源：http://hz.jinghuilouyu.cn/gtfkxjxtfd.html

void inc(int &x) { ++x; }
来源：http://hz.c1oappe.top/gtojzholye.html

[S45] C++：lambda
来源：http://hz.cdnleiting.top/gtgdsiqsny.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinyuanbaomall.cn/gtrbqqlhbs.html

[S46] C++：函数模板
来源：http://hz.jlsjyb.cn/gtwheagwag.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnqzz.top/gtjhgoduba.html

[S47] C++：结构化绑定遍历
来源：http://hz.nanxinkj.top/gtpqfopvin.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cashguo.top/gtibmzgsgy.html

[S48] C++：逐行读文件
来源：http://hz.sxryk.cn/gtgkaapano.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tanke756.top/gtumdkppnf.html

while (std::getline(in, line)) { }
来源：http://hz.jianghu66.top/gtuzkiexkj.html

[S49] C++：写文件
来源：http://hz.hywenlv.cn/gtiffsgynz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ehwqpu.com/gtyjkjoqgp.html

[S50] C++：格式化数字
来源：http://hz.yuxming.cn/gtluovwnhj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yuxming.cn/gttfqxhdlc.html

[S51] C++：显式类型转换
来源：http://hz.hongshengwenyu.top/gtdhsxdgbg.html

static_cast<double>(a) / b
来源：http://hz.haohaochexian.top/gtzbyxjari.html

[S52] C++：const 与 noexcept
来源：http://hz.xuanzx.com/gtszrxfngh.html

int size() const noexcept { return n_; }
来源：http://hz.kuanghao11.cn/gtpocipzyw.html

[S53] C++：移动语义
来源：http://hz.bjfxy.top/gtmhkvbbfr.html

std::vector<int> w = std::move(v);
来源：http://hz.hysaishi.cn/gtdbmzzrlj.html

[S54] C++：异常处理
来源：http://hz.jyoumei.cn/gtubsixbob.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nanxinkj.top/gtpctnwsul.html

[S55] C++：结构化绑定
来源：http://hz.yangfankeji.com/gtjqjldxip.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.316326.xyz/gtwfjbzfav.html

[S56] C++：optional
来源：http://hz.chenjidiqi.icu/gtyxdfjpht.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.havefunace.top/gtljodrqsq.html

[S57] C++：编译期常量
来源：http://hz.xuanzx.com/gtowfsojfn.html

constexpr int N = 10;
来源：http://hz.chenzaomai.com/gtrjqbbnrj.html

[S58] C++：命名空间
来源：http://hz.yonumen.top/gtlbbjeuth.html

namespace ns { int f() { return 1; } }
来源：http://hz.ppjwa.cn/gtwgsmufhw.html

[S59] C++：静态断言
来源：http://hz.sweek.top/gtafcvdlyt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenzaomai.com/gtypacpvsb.html

[S60] C++：遍历并删除元素
来源：http://hz.jlsjyb.cn/gtgbgwmrjk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ydjk.org.cn/gtrwooyemi.html

================================================================================
来源：http://hz.cqqwz.cn/gttuaspllg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hongshengwenyu.top/gtzlsunfyu.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtmvaxgkjm.html

[T01] Kotlin：Hello World
来源：http://hz.xziqi.cn/gtdsknilwq.html

println("Hello")
来源：http://hz.daria6918.cn/gtstyhdpqw.html

[T02] Kotlin：变量
来源：http://hz.jinqigfzy.top/gtmvdyxagx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.smart0.xyz/gtodviqxqc.html

[T03] Kotlin：字符串模板
来源：http://hz.ydzc1.top/gtlnuflcqx.html

"值: $b"
来源：http://hz.xylfe.cn/gtafcvaozj.html

[T04] Kotlin：空安全
来源：http://hz.zycfv.cn/gtzfmixbsa.html

val n: String? = null;  n?.length
来源：http://hz.daxiang520.top/gtbwlllzrt.html


<!-- 参考信息 -->