代发 wailian999

name="${1:-default}"
来源：http://hz.hywenlv.cn/gtjcczccsn.html

[R06] 判断命令是否存在
来源：http://hz.tian-w.cn/gtbuajljuk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hnxiangtu.top/gtzpxjrqmk.html

[R07] if 判断文件
来源：http://hz.jinghuilouyu.cn/gtuqgitrlf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shanyushiyangkeji.top/gtrvagrtlz.html

[R08] 数值比较
来源：http://hz.dashuyun.cn/gtwwqdaqsz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.316326.xyz/gtpovpvhky.html

[R09] 字符串比较
来源：http://hz.ydzc1.top/gtuumseizh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hongshengwenyu.top/gtgrtfftce.html

[R10] 正则匹配
来源：http://hz.daria6918.cn/gtbbyxogoz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.fengsongda.top/gtcigwjghs.html

[R11] case 多分支
来源：http://hz.zhijiandao.cn/gtkmzgnfak.html

case "$1" in
来源：http://hz.yueranfly.top/gtjdstsbsn.html

start) echo "启动" ;;
来源：http://hz.svipenyu.cn/gtzxiwafkz.html

stop)  echo "停止" ;;
来源：http://hz.yj202588.top/gtpybviqwn.html

*)     echo "未知命令" ;;
来源：http://hz.feifeiyinyue.top/gtnoqcjqey.html

esac
来源：http://hz.c1oappe.top/gtusmmvcrc.html

[R12] for 遍历文件
来源：http://hz.xylfe.cn/gtfainuwxx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.feifeiyinyue.top/gtdohlfffp.html

[R13] for 计数循环
来源：http://hz.zhijiandao.cn/gtcdtrlapr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.9152youxi.cn/gtluxwftsq.html

[R14] C 风格 for
来源：http://hz.daxiang520.top/gtaoomblsl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ydjk.org.cn/gtaetqrvsu.html

[R15] while 逐行读文件
来源：http://hz.sufxvd.cn/gtnysupgfs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xziqi.cn/gtcoxfpzdi.html

[R16] until 等待条件
来源：http://hz.jiagoushi.top/gttujnpvpz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ydzc1.top/gtbsxfnfkc.html

[R17] 数组定义与取值
来源：http://hz.yonumen.top/gtcgkezsia.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinghuilouyu.cn/gtkrblvscp.html

[R18] 遍历数组
来源：http://hz.mhx1999.top/gtzyqplsrc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.bjfxy.top/gthylbkoze.html

[R19] 数组长度
来源：http://hz.nanxuanxn.top/gtnysndhfw.html

echo "${#arr[@]}"
来源：http://hz.tianlin.xyz/gtjzozmsww.html

[R20] 关联数组（字典）
来源：http://hz.zhaomingkeji.xyz/gtmdlyugnv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nanxuanxn.top/gtyhogftky.html

[R21] 字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtbvuibdrz.html

echo "${#s}"
来源：http://hz.52xcode.cn/gtymseqmkp.html

[R22] 截取子串
来源：http://hz.zhiwuduotai.top/gtgqxjlzlw.html

echo "${s:0:5}"
来源：http://hz.yuxming.cn/gtzyxofygo.html

[R23] 字符串替换
来源：http://hz.redwolf501.top/gtqjltlytk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.birdmap.top/gtbtjoozbl.html

[R24] 大小写转换
来源：http://hz.mhx1999.top/gtnvbgymle.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jqgufenzy.top/gtqdceosog.html

[R25] 去后缀 / 去前缀
来源：http://hz.xuetiantiany.cn/gtutvhawso.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.daxiang520.top/gtwhfcpill.html

[R26] 命令替换
来源：http://hz.tanke756.top/gtknhewvdd.html

now=$(date +%F); echo "$now"
来源：http://hz.jlsjyb.cn/gtgjqtgbqd.html

[R27] 算术展开
来源：http://hz.sweek.top/gtynaaugam.html

echo $((1 + 2 * 3))
来源：http://hz.hongshengwenyu.top/gtmwnlviss.html

[R28] 浮点运算
来源：http://hz.yongpay.top/gtqaxnshou.html

echo "scale=2; 10/3" | bc
来源：http://hz.yongpay.top/gtclkhsdyb.html

[R29] 定义函数
来源：http://hz.yuanzhike.top/gtohwnoajb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.wangshuangyany.cn/gtbxrurdet.html

[R30] 函数返回状态码
来源：http://hz.cucudq.cn/gtagqqnjmf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.iojbl.cn/gtakbdbehl.html

[R31] 局部变量
来源：http://hz.smart0.xyz/gtyvhosqzt.html

f() { local x=1; echo "$x"; }
来源：http://hz.hysaishi.cn/gtdiccdhdc.html

[R32] 参数个数校验
来源：http://hz.jinqigufen.top/gtfgwppmwr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yanxiufei.cn/gtfcmlourj.html

[R33] 捕获错误并提示行号
来源：http://hz.pycfn.com/gtjeagdeld.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jiagoushi.top/gtqamdzffg.html

[R34] 退出时清理
来源：http://hz.zhongyouzk.top/gtmyrlxjwo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnqzz.top/gtnreoxzvy.html

[R35] 后台执行并等待
来源：http://hz.cucudq.cn/gtqmsrxtvy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yueranfly.top/gtaucxgesy.html

[R36] 并发执行多个任务
来源：http://hz.nwbrower.top/gtpaaergze.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.quarkkingdee.top/gtrtkrambj.html

[R37] 把输出赋给变量
来源：http://hz.zhaomingkeji.xyz/gttfuqsgtn.html

files=$(ls -1)
来源：http://hz.fengsongda.top/gtolfyajvk.html

[R38] 管道串联
来源：http://hz.zhiwuduotai.top/gtncfzysnf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.iojbl.cn/gtvmttxrfy.html

[R39] 重定向标准输出与错误
来源：http://hz.yongpay.top/gtygonfpyn.html

cmd > out.log 2>&1
来源：http://hz.xylfe.cn/gtuendtagc.html

[R40] 追加写日志
来源：http://hz.daxiang520.top/gtwmmvhjmr.html

echo "log" >> out.log
来源：http://hz.sufxvd.cn/gtvhgotmza.html

[R41] 丢弃输出
来源：http://hz.nanxuanxn.top/gthcexxljq.html

cmd >/dev/null 2>&1
来源：http://hz.cdnleiting.top/gtdfackosd.html

[R42] 输入重定向
来源：http://hz.ivvv.top/gteobkickd.html

wc -l < a.txt
来源：http://hz.yangfankeji.com/gtjonkukmh.html

[R43] 按名字查找文件
来源：http://hz.snrcjt.cn/gtrfinrksi.html

find . -name "*.log" -type f
来源：http://hz.haohaochexian.top/gtaujibges.html

[R44] 按修改时间查找
来源：http://hz.cdnleiting.top/gtjxrxtntk.html

find . -mtime -7 -type f
来源：http://hz.yvedp.cn/gtpzvrfceb.html

[R45] 批量删除
来源：http://hz.hammf.cn/gttvvovycm.html

find . -name "*.tmp" -delete
来源：http://hz.yongpay.top/gtfugctutg.html

[R46] 递归替换文件内容
来源：http://hz.hammf.cn/gthxvnoptf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.mhx1999.top/gtkaxnbymv.html

[R47] sed 单行替换
来源：http://hz.cqqwz.cn/gtnjaoqkfi.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xylfe.cn/gthwzeyzgw.html

[R48] awk 取指定列
来源：http://hz.ehwqpu.com/gtetgtvogv.html

awk '{print $1, $3}' a.txt
来源：http://hz.hysaishi.cn/gtpwunymyp.html

[R49] awk 带条件
来源：http://hz.nwbrower.top/gtresbistf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xziqi.cn/gtbsbuadzu.html

[R50] awk 求和
来源：http://hz.hongshengwenyu.top/gtxjhkwdty.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.316326.xyz/gtbkhvfcpy.html

[R51] 排序去重取前几
来源：http://hz.meibo888.top/gtyipejcza.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tianlin.xyz/gtultcdprm.html

[R52] 统计行数
来源：http://hz.pengpengdd.cyou/gtsnonyzgb.html

wc -l a.txt
来源：http://hz.vqdsnc.cn/gtdlqwbwpk.html

[R53] 查看文件头与实时尾
来源：http://hz.yvedp.cn/gthsewosgm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.0kj1m.cn/gtyjmzomtf.html

[R54] 比较两个文件
来源：http://hz.bjfxy.top/gtgspngibv.html

diff a.txt b.txt
来源：http://hz.jqgfzy.top/gtubgemitn.html

[R55] 压缩与解压
来源：http://hz.nanxuanxn.top/gtqjolndyt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shzxlz.cn/gtmohciape.html

[R56] 远程拷贝
来源：http://hz.xinyue.icu/gtvsvncjad.html

scp file user@host:/path/
来源：http://hz.gotoacloud.top/gtsyntszdm.html

[R57] 远程执行命令
来源：http://hz.wangdashe.top/gtpofekbae.html

ssh user@host 'uptime'
来源：http://hz.jianghu66.top/gtbetivbre.html

[R58] 下载文件
来源：http://hz.xinyue.icu/gtkcnblidb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nanxuanxn.top/gtnsyyrhwf.html

[R59] 发 POST JSON
来源：http://hz.yuanzhike.top/gtutawfdnu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.havefunace.top/gtsoiebrcl.html

[R60] 只看 HTTP 状态码
来源：http://hz.cucudq.cn/gtwkljidzk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cucudq.cn/gthxmqrhce.html

[R61] 磁盘占用
来源：http://hz.zhongyouzk.top/gtaxxsvusv.html

df -h;  du -sh *
来源：http://hz.jyoumei.cn/gtkrsqecur.html

[R62] 找最占空间的文件
来源：http://hz.jqgufenzy.top/gtejdbjfov.html

du -ah . | sort -rh | head -10
来源：http://hz.iojbl.cn/gtciwkimxw.html

[R63] 内存与进程
来源：http://hz.pycfn.com/gtwvkgcygt.html

free -h;  ps aux | grep nginx
来源：http://hz.cheryme.top/gtqvlwpndh.html

[R64] 结束进程
来源：http://hz.hammf.cn/gtswjudqhp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jqgufenzy.top/gthzfzogyn.html

[R65] 查看端口占用
来源：http://hz.svipenyu.cn/gtldjuxwqd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhijiandao.cn/gtfjwcbxnv.html

[R66] 定时任务
来源：http://hz.tanke756.top/gtopozqzno.html

crontab -e;  crontab -l
来源：http://hz.cheryme.top/gtbmlrczdw.html

[R67] 生成随机十六进制串
来源：http://hz.gogol.net.cn/gtmbuzbdme.html

openssl rand -hex 16
来源：http://hz.xuanzx.com/gtxrlmpxjc.html

[R68] 计算文件校验值
来源：http://hz.tian-w.cn/gtekuvwuul.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ppjwa.cn/gthmzafaxd.html

[R69] 生成随机密码
来源：http://hz.cqqwz.cn/gtahbtufvh.html

head -c 16 /dev/urandom | base64
来源：http://hz.tian-w.cn/gtoyszbele.html

[R70] 时间戳与互转
来源：http://hz.zhengqikj.top/gtdzyiziol.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258888.top/gtpoiinkma.html

[R71] 日期格式化
来源：http://hz.yj20258.top/gtoizgsumk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.iojbl.cn/gtynhelcmx.html

[R72] 等待端口就绪
来源：http://hz.zdqjudy.top/gteyiiyxef.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jianghu66.top/gthsyarxbc.html

[R73] 分割大日志
来源：http://hz.xuetiantiany.cn/gtmwncaaap.html

split -l 1000 big.log part_
来源：http://hz.yuanzhike.top/gtpnqayrpr.html

[R74] 批量重命名
来源：http://hz.snrcjt.cn/gtlwprfitu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.wangshuangyany.cn/gtiohbizur.html

[R75] 导出环境变量
来源：http://hz.jlsjyb.cn/gtjihswazq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.52xcode.cn/gtpmpidwab.html

[R76] 使用临时文件
来源：http://hz.cheryme.top/gtfjexasbx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shuidangran.top/gtfhjtagtn.html

[R77] 读取用户输入
来源：http://hz.52xcode.cn/gtvutmcqnd.html

read -rp "请输入: " ans
来源：http://hz.zhoulong.xyz/gtqhxfptil.html

[R78] 交互式菜单
来源：http://hz.xylfe.cn/gtpeymzugp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sweek.top/gtyeaqbzuo.html

[R79] 解析命令行选项
来源：http://hz.tianlin.xyz/gtwfhvsiib.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.nanxuanxn.top/gtczptjkib.html

[R80] 查看脚本执行耗时
来源：http://hz.xziqi.cn/gtetuqhqyj.html

time ./run.sh
来源：http://hz.hammf.cn/gtmrvkquio.html

================================================================================
来源：http://hz.gzhubu.top/gtnkfkpojt.html

S. C / C++ 专题
来源：http://hz.daxiang520.top/gtzfxzyrzk.html

================================================================================
来源：http://hz.smart0.xyz/gtrrrtqivv.html

[S01] C：Hello World
来源：http://hz.chenzaomai.com/gtrznjooax.html

#include <stdio.h>
来源：http://hz.cdnleiting.top/gtlcabugwj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hysaishi.cn/gtvmynqvui.html

[S02] C：变量与格式化输出
来源：http://hz.hnqzz.top/gteglfqmtd.html

int a = 10; printf("%d\n", a);
来源：http://hz.shzxlz.cn/gtelsqtmjs.html

[S03] C：读入整数
来源：http://hz.fengsongda.top/gtsmwbvypn.html

int x; scanf("%d", &x);
来源：http://hz.sxryk.cn/gtzdbbucxz.html

[S04] C：字符串复制
来源：http://hz.fzhhl.top/gtnyshltcp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sysykeji.top/gtwlmlqqtn.html

[S05] C：字符串长度
来源：http://hz.meibo888.top/gtavuwjhcg.html

strlen(s)
来源：http://hz.hysaishi.cn/gtiwsmlqte.html

[S06] C：字符串比较
来源：http://hz.daria6918.cn/gtplkbwegs.html

strcmp(a, b) == 0
来源：http://hz.cdnleiting.top/gtzhsskugn.html

[S07] C：数组遍历求和
来源：http://hz.snrcjt.cn/gtncvjsahc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cashguo.top/gtnhgtryyl.html

[S08] C：动态内存分配与释放
来源：http://hz.xingfuxueyuan.xyz/gtjdlnhzov.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cheryme.top/gtaeogzkvt.html

[S09] C：结构体定义与初始化
来源：http://hz.shuidangran.top/gtpnltlurp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zycfv.cn/gtqhlofeho.html

[S10] C：指针与解引用
来源：http://hz.yueranfly.top/gtrqpzfpnj.html

int *p = &a;  *p = 5;
来源：http://hz.zhijiandao.cn/gtnbqnjamm.html

[S11] C：逐行读文件
来源：http://hz.zhiwuduotai.top/gtjfiapmwx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yonumen.top/gtyjeoplaz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hammf.cn/gtsytorpsl.html

fclose(f);
来源：http://hz.sysykeji.top/gtnfmbcgkj.html

[S12] C：写文件
来源：http://hz.yangfankeji.com/gtabhqypbd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.svipenyu.cn/gtmnmhalua.html

[S13] C：宏定义
来源：http://hz.aibaodan.cn/gtnzrwkbuh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.havefunace.top/gtprteorop.html

[S14] C：枚举
来源：http://hz.xylfe.cn/gthshculka.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhengqikj.top/gtzhtowiow.html

[S15] C：类型转换
来源：http://hz.meibo888.top/gtcpxxxhns.html

(double) a / b
来源：http://hz.yuxming.cn/gtwxkvsajw.html

[S16] C：位操作置位
来源：http://hz.hammf.cn/gtfiulpace.html

x |= (1 << 3);
来源：http://hz.jinqigfzy.top/gtrbgxnvki.html

[S17] C：安全拼接字符串
来源：http://hz.zhongyouzk.top/gtkoopthro.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhijiandao.cn/gtsokeklfg.html

[S18] C：命令行参数
来源：http://hz.jinyuanbaomall.cn/gtukxnbhkv.html

int main(int argc, char **argv)
来源：http://hz.zhongyouzk.top/gtelflnbvc.html

[S19] C：快速排序
来源：http://hz.nanxinkj.top/gtbufvikjv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cdnleiting.top/gtjcxjhqoy.html

[S20] C：二分查找
来源：http://hz.cqqwz.cn/gtaenkbabd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hnqzz.top/gtwwdkmfoz.html

[S21] C：字符类别判断
来源：http://hz.yj20258888.top/gtllybkest.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xylfe.cn/gtobgxdcns.html

[S22] C：字符串转数字
来源：http://hz.gogol.net.cn/gtfxrpmcbd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.snrcjt.cn/gtfaiskrgk.html

[S23] C：随机数
来源：http://hz.aibaodan.cn/gttpjwejow.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jiagoushi.top/gtwznynyol.html

[S24] C：获取本地时间
来源：http://hz.yuanzhike.top/gtlafvpast.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sysykeji.top/gtxcvufkzo.html

[S25] C：内存拷贝
来源：http://hz.feifeiyinyue.top/gtlvamigbx.html

memcpy(dst, src, n);
来源：http://hz.chenzaomai.com/gtjnrvovdi.html

[S26] C：内存清零
来源：http://hz.yanxiufei.cn/gtorvhkqml.html

memset(a, 0, sizeof a);
来源：http://hz.zycfv.cn/gtdnnamtcs.html

[S27] C：定义常量
来源：http://hz.hammf.cn/gtljlyxxgn.html

const double PI = 3.14159;
来源：http://hz.chenlongwang.top/gtrrkmthgx.html

[S28] C：静态变量
来源：http://hz.aibaodan.cn/gtroodqwjz.html

static int counter = 0;
来源：http://hz.zhongyouzk.top/gtrifnjvjn.html

[S29] C：变参函数
来源：http://hz.quarkkingdee.top/gthouzzidj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jianghu66.top/gtoeawxjft.html

[S30] C：头文件保护
来源：http://hz.yuanzhike.top/gtavrtzfns.html

#ifndef X_H
来源：http://hz.andypj.xyz/gtaihlsrdb.html

#define X_H
来源：http://hz.sufxvd.cn/gtzlooegye.html

#endif
来源：http://hz.gotoacloud.top/gtrsxhvipw.html

[S31] C++：Hello World
来源：http://hz.guannengcc.top/gtwnebzxxn.html

#include <iostream>
来源：http://hz.shangyingyoupin.top/gtjrtfslli.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.pycfn.com/gtwyhsbwnm.html

[S32] C++：字符串
来源：http://hz.hnxiangtu.top/gtbvyofxpa.html

std::string s = "hi";  s += "!";
来源：http://hz.bjfxy.top/gtjhxbswly.html

[S33] C++：vector 增删
来源：http://hz.zhixingplan.top/gtimvlgkjx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xingfuxueyuan.xyz/gtxnwcidhy.html

[S34] C++：遍历 vector
来源：http://hz.shanyushiyangtech.top/gttwbjdzup.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sweek.top/gtbmuuldps.html

[S35] C++：map
来源：http://hz.cheryme.top/gtctrcxekx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cdnleiting.top/gtjnnlwwxw.html

[S36] C++：unordered_map
来源：http://hz.ywan-chungtsiang.top/gtlknnzgxb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yangfankeji.com/gtzwxghris.html

[S37] C++：set
来源：http://hz.9152youxi.cn/gtrjujujba.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.havefunace.top/gtztftakxv.html

[S38] C++：排序
来源：http://hz.tian-w.cn/gtxitgpzkf.html

std::sort(v.begin(), v.end());
来源：http://hz.redwolf501.top/gthirqmxwb.html

[S39] C++：自定义比较器排序
来源：http://hz.shanyushiyangkeji.top/gtrupudkcx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ydzc1.top/gtmbwislkt.html

[S40] C++：查找元素
来源：http://hz.gaohongyu789.top/gtivdoplsv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.dianchejie.cn/gtqorwtpwm.html

[S41] C++：类与构造函数
来源：http://hz.meibo888.top/gtqcisbzqu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cashguo.top/gtsugsbauu.html

[S42] C++：继承与虚函数
来源：http://hz.yueranfly.top/gtithacdwm.html

class B : public Base { public: void f() override {} };
来源：http://hz.jiagoushi.top/gteetfjqzd.html

[S43] C++：智能指针
来源：http://hz.yonumen.top/gtnvflomru.html

auto p = std::make_unique<int>(5);
来源：http://hz.0kj1m.cn/gtqjgousrn.html

[S44] C++：引用传参
来源：http://hz.zhengqikj.top/gtgjjjjoey.html

void inc(int &x) { ++x; }
来源：http://hz.pycfn.com/gtjnldbnqo.html

[S45] C++：lambda
来源：http://hz.tianlin.xyz/gtvbozehss.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xylfe.cn/gtwiqiavhg.html

[S46] C++：函数模板
来源：http://hz.feifeiyinyue.top/gtxfgdasve.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xuanzx.com/gtkdjuyrmd.html

[S47] C++：结构化绑定遍历
来源：http://hz.shangyingyoupin.top/gtrdloklzb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sxryk.cn/gtqwcqwigb.html

[S48] C++：逐行读文件
来源：http://hz.yj20258.top/gtiurzhipp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shanyushiyangkeji.top/gtcvvawwlh.html

while (std::getline(in, line)) { }
来源：http://hz.ehwqpu.com/gtcckcpdxe.html

[S49] C++：写文件
来源：http://hz.sxryk.cn/gtqibgfmkm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cqqwz.cn/gtnianxoqb.html

[S50] C++：格式化数字
来源：http://hz.cheryme.top/gtggcenjol.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenjidiqi.icu/gtunnjuedm.html

[S51] C++：显式类型转换
来源：http://hz.zhijiandao.cn/gtldmbrbjn.html

static_cast<double>(a) / b
来源：http://hz.iojbl.cn/gtofbuifqs.html

[S52] C++：const 与 noexcept
来源：http://hz.hnxiangtu.top/gtllkmvmql.html

int size() const noexcept { return n_; }
来源：http://hz.wangdashe.top/gtfjunusre.html

[S53] C++：移动语义
来源：http://hz.zycfv.cn/gtuwrnibhs.html

std::vector<int> w = std::move(v);
来源：http://hz.iojbl.cn/gthsbgcnnp.html

[S54] C++：异常处理
来源：http://hz.havefunace.top/gtgjbtuzim.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yonumen.top/gtcbcjtzuw.html

[S55] C++：结构化绑定
来源：http://hz.316326.xyz/gtbcvdptyn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinyuanbaomall.cn/gtggcaepem.html

[S56] C++：optional
来源：http://hz.hongshengwenyu.top/gtcaczvmmp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jyoumei.cn/gtyjixwejd.html

[S57] C++：编译期常量
来源：http://hz.gaohongyu789.top/gtkwqxvhid.html

constexpr int N = 10;
来源：http://hz.gaohongyu789.top/gtgocyzrin.html

[S58] C++：命名空间
来源：http://hz.hfpthk.cn/gtlsbkvosq.html

namespace ns { int f() { return 1; } }
来源：http://hz.jqgufenzy.top/gtjtroioyt.html

[S59] C++：静态断言
来源：http://hz.hnxiangtu.top/gtnwjjtqhh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shanyushiyangtech.top/gtkifsohuq.html

[S60] C++：遍历并删除元素
来源：http://hz.jqgufenzy.top/gtkeqjuohh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ydjk.org.cn/gtuhplgvgd.html

================================================================================
来源：http://hz.dashuyun.cn/gtlonxqwbc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.redwolf501.top/gtmtqzmbwn.html

================================================================================
来源：http://hz.chenzaomai.com/gtydcdtuuq.html

[T01] Kotlin：Hello World
来源：http://hz.hnqzz.top/gtrqpmenxd.html

println("Hello")
来源：http://hz.bjfxy.top/gtuzshzbsx.html

[T02] Kotlin：变量
来源：http://hz.vqdsnc.cn/gtvavjyxgi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sysykeji.top/gtsgbkqhzo.html

[T03] Kotlin：字符串模板
来源：http://hz.yvedp.cn/gtcssfxwoa.html

"值: $b"
来源：http://hz.jinqigufen.top/gtkutwwdyh.html

[T04] Kotlin：空安全
来源：http://hz.havefunace.top/gtsidittss.html

val n: String? = null;  n?.length
来源：http://hz.yvedp.cn/gtqfgjmqgj.html

[T05] Kotlin：when 表达式
来源：http://hz.gaohongyu789.top/gtjhzsynhj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.bjfxy.top/gtycxrstei.html

[T06] Kotlin：集合映射
来源：http://hz.sweek.top/gtvmmbnmmz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.316326.xyz/gthwuvddtz.html


<!-- 参考信息 -->