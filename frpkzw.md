代发 wailian999

set -euo pipefail
来源：http://hz.gzhubu.top/gtgkukjxmj.html

[R02] 变量赋值与使用
来源：http://hz.bjfxy.top/gtwtjjpyhm.html

name="Tom"; echo "$name"
来源：http://hz.quarkkingdee.top/gtbtvlzqsi.html

[R03] 只读变量
来源：http://hz.zycfv.cn/gtpbarysbp.html

readonly PI=3.14
来源：http://hz.gogol.net.cn/gtjbxtbtxu.html

[R04] 位置参数
来源：http://hz.jinqigufen.top/gtfqoprpfg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.52xcode.cn/gtgtraapeh.html

[R05] 参数默认值
来源：http://hz.zycfv.cn/gtwqeilalg.html

name="${1:-default}"
来源：http://hz.pengpengdd.cyou/gtozxcethn.html

[R06] 判断命令是否存在
来源：http://hz.pengpengdd.cyou/gtojwfjrok.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jianghu66.top/gtzxxucvvp.html

[R07] if 判断文件
来源：http://hz.zhixingplan.top/gtdgkdelmf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ehwqpu.com/gtybmuhfxj.html

[R08] 数值比较
来源：http://hz.zycfv.cn/gtmvpcepuc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yonumen.top/gtijntzezh.html

[R09] 字符串比较
来源：http://hz.zhixingplan.top/gtmjscbwun.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tianlin.xyz/gtvcsyluuo.html

[R10] 正则匹配
来源：http://hz.chenzaomai.com/gtucyrvlzc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hnxiangtu.top/gtsrwphcee.html

[R11] case 多分支
来源：http://hz.sufxvd.cn/gtbyjmrcee.html

case "$1" in
来源：http://hz.52xcode.cn/gtuuqocvrk.html

start) echo "启动" ;;
来源：http://hz.zhongyouzk.top/gtvsrygwap.html

stop)  echo "停止" ;;
来源：http://hz.vqdsnc.cn/gtyqbzksgj.html

*)     echo "未知命令" ;;
来源：http://hz.cqqwz.cn/gtpzjtwiar.html

esac
来源：http://hz.tianlin.xyz/gtchkrgdzq.html

[R12] for 遍历文件
来源：http://hz.pengpengdd.cyou/gtkpphxszz.html

for f in *.txt; do echo "$f"; done
来源：http://hz.wangdashe.top/gtplgbbern.html

[R13] for 计数循环
来源：http://hz.kuanghao11.cn/gthnsgzzwz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tian-w.cn/gtipzlagph.html

[R14] C 风格 for
来源：http://hz.chenjidiqi.icu/gtucymotij.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.bjfxy.top/gtvhvtctgp.html

[R15] while 逐行读文件
来源：http://hz.xziqi.cn/gtqkbrqsfq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhiwuduotai.top/gtehlrkwdf.html

[R16] until 等待条件
来源：http://hz.shanyushiyangkeji.top/gtjngiwurk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.vqdsnc.cn/gtnhltsvng.html

[R17] 数组定义与取值
来源：http://hz.hongshengwenyu.top/gtcpchjddt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.0kj1m.cn/gtvwoqlnzt.html

[R18] 遍历数组
来源：http://hz.cucudq.cn/gtuocpkitd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.mhx1999.top/gtthivohtb.html

[R19] 数组长度
来源：http://hz.ivvv.top/gtmvidwnxn.html

echo "${#arr[@]}"
来源：http://hz.zhaomingkeji.xyz/gthreevfzg.html

[R20] 关联数组（字典）
来源：http://hz.jianghu66.top/gthtcqxosf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ivvv.top/gtpootiige.html

[R21] 字符串长度
来源：http://hz.dianchejie.cn/gtzkwhkkbp.html

echo "${#s}"
来源：http://hz.aizwys.cn/gtuwlnibvy.html

[R22] 截取子串
来源：http://hz.meibo888.top/gtwdxgdszt.html

echo "${s:0:5}"
来源：http://hz.aizwys.cn/gtyrctsdwy.html

[R23] 字符串替换
来源：http://hz.wangshuangyany.cn/gtidtfqjxo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yanxiufei.cn/gtoswbzqse.html

[R24] 大小写转换
来源：http://hz.zycfv.cn/gtqubowlja.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xuanzx.com/gtalcybisg.html

[R25] 去后缀 / 去前缀
来源：http://hz.zycfv.cn/gtktabwpdh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hywenlv.cn/gtizhgauyd.html

[R26] 命令替换
来源：http://hz.shzxlz.cn/gtwcvgtind.html

now=$(date +%F); echo "$now"
来源：http://hz.yangfankeji.com/gtybwonnce.html

[R27] 算术展开
来源：http://hz.zhijiandao.cn/gtqffnbldi.html

echo $((1 + 2 * 3))
来源：http://hz.svipenyu.cn/gtjapdyier.html

[R28] 浮点运算
来源：http://hz.shzxlz.cn/gtzzxaufpb.html

echo "scale=2; 10/3" | bc
来源：http://hz.ivvv.top/gtxjyyoobo.html

[R29] 定义函数
来源：http://hz.redwolf501.top/gtqsqtykjf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jqgfzy.top/gtbrfoqspr.html

[R30] 函数返回状态码
来源：http://hz.shuidangran.top/gtqigkytil.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.fengsongda.top/gtflfefxtn.html

[R31] 局部变量
来源：http://hz.tanke756.top/gtrauyisqr.html

f() { local x=1; echo "$x"; }
来源：http://hz.gaohongyu789.top/gtknsjhzck.html

[R32] 参数个数校验
来源：http://hz.andypj.xyz/gtgzolvahg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cucudq.cn/gtrgtwfyhq.html

[R33] 捕获错误并提示行号
来源：http://hz.ywan-chungtsiang.top/gtkaefhxai.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tian-w.cn/gtndqrtfyx.html

[R34] 退出时清理
来源：http://hz.yj202588.top/gtssgsrsvj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ehwqpu.com/gtsjybrqgu.html

[R35] 后台执行并等待
来源：http://hz.chenzaomai.com/gtsbobmnsq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhoulong.xyz/gtlzeefhxc.html

[R36] 并发执行多个任务
来源：http://hz.xziqi.cn/gtjlaqosfl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gogol.net.cn/gtojilzqoo.html

[R37] 把输出赋给变量
来源：http://hz.yuxming.cn/gtgvhanssv.html

files=$(ls -1)
来源：http://hz.sysykeji.top/gtsmwqaxoc.html

[R38] 管道串联
来源：http://hz.zhengqikj.top/gthkpqqszc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.feifeiyinyue.top/gthxzijeyy.html

[R39] 重定向标准输出与错误
来源：http://hz.hnxiangtu.top/gtzmhcpzgq.html

cmd > out.log 2>&1
来源：http://hz.tian-w.cn/gtnddfzbzu.html

[R40] 追加写日志
来源：http://hz.shuidangran.top/gtqddkgvrt.html

echo "log" >> out.log
来源：http://hz.cdnleiting.top/gtfeainslu.html

[R41] 丢弃输出
来源：http://hz.c1oappe.top/gtwybtkxhz.html

cmd >/dev/null 2>&1
来源：http://hz.cheryme.top/gtkhuviwpw.html

[R42] 输入重定向
来源：http://hz.svipenyu.cn/gtriwistxn.html

wc -l < a.txt
来源：http://hz.hnxiangtu.top/gtuviqvkrg.html

[R43] 按名字查找文件
来源：http://hz.smart0.xyz/gttzifthih.html

find . -name "*.log" -type f
来源：http://hz.yj20258888.top/gtnmksnsnh.html

[R44] 按修改时间查找
来源：http://hz.tianlin.xyz/gtcmflembx.html

find . -mtime -7 -type f
来源：http://hz.hfpthk.cn/gttrbtegox.html

[R45] 批量删除
来源：http://hz.fzhhl.top/gtkldgitbt.html

find . -name "*.tmp" -delete
来源：http://hz.gzhubu.top/gtertzdhzj.html

[R46] 递归替换文件内容
来源：http://hz.zhongyouzk.top/gtniruyxqy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.52xcode.cn/gtkcljsjas.html

[R47] sed 单行替换
来源：http://hz.kuanghao11.cn/gtlbabcjol.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zdqjudy.top/gtcqauisbe.html

[R48] awk 取指定列
来源：http://hz.xingfuxueyuan.xyz/gtxqrrtnvm.html

awk '{print $1, $3}' a.txt
来源：http://hz.smart0.xyz/gtukjjgrgy.html

[R49] awk 带条件
来源：http://hz.zhongyouzk.top/gtusxjyjya.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.pycfn.com/gtlleresxc.html

[R50] awk 求和
来源：http://hz.svipenyu.cn/gtxtwpfikx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xuanzx.com/gtyupwkexw.html

[R51] 排序去重取前几
来源：http://hz.zhaomingkeji.xyz/gtfghhwyna.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.52xcode.cn/gtesgoxzjx.html

[R52] 统计行数
来源：http://hz.sufxvd.cn/gtuiolzlrx.html

wc -l a.txt
来源：http://hz.sxryk.cn/gtyymcrqtx.html

[R53] 查看文件头与实时尾
来源：http://hz.yuxming.cn/gtelqsnapf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.bjfxy.top/gtllmexgis.html

[R54] 比较两个文件
来源：http://hz.jqgufenzy.top/gtywqzehaw.html

diff a.txt b.txt
来源：http://hz.ybcxt.top/gtlcygbjwv.html

[R55] 压缩与解压
来源：http://hz.jianghu66.top/gtpfvjwdfu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ywan-chungtsiang.top/gtmdczppjo.html

[R56] 远程拷贝
来源：http://hz.chenjidiqi.icu/gtyozfacld.html

scp file user@host:/path/
来源：http://hz.ydjk.org.cn/gtglckizgv.html

[R57] 远程执行命令
来源：http://hz.gzhubu.top/gtkncwakms.html

ssh user@host 'uptime'
来源：http://hz.zhixingplan.top/gtgrgxzxri.html

[R58] 下载文件
来源：http://hz.xuanzx.com/gtjhnbgjag.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ybcxt.top/gtqfnpzmpw.html

[R59] 发 POST JSON
来源：http://hz.ydzc1.top/gtxdosctzl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhaomingkeji.xyz/gtiypyohyi.html

[R60] 只看 HTTP 状态码
来源：http://hz.zdqjudy.top/gtkyjpegmv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yanxiufei.cn/gtltakjbvg.html

[R61] 磁盘占用
来源：http://hz.shanyushiyangtech.top/gtbiuflwxs.html

df -h;  du -sh *
来源：http://hz.chenjidiqi.icu/gtcddgwkuu.html

[R62] 找最占空间的文件
来源：http://hz.guannengcc.top/gtkmfrbhcx.html

du -ah . | sort -rh | head -10
来源：http://hz.tanke756.top/gtofsxzmuf.html

[R63] 内存与进程
来源：http://hz.chenzaomai.com/gtenaluetm.html

free -h;  ps aux | grep nginx
来源：http://hz.meibo888.top/gtrlppoefw.html

[R64] 结束进程
来源：http://hz.yonumen.top/gtpuswomoa.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hysaishi.cn/gtbdinenyx.html

[R65] 查看端口占用
来源：http://hz.ehwqpu.com/gtzipjzkxi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hongshengwenyu.top/gtjkqiclmr.html

[R66] 定时任务
来源：http://hz.yangfankeji.com/gtjiwpwmfb.html

crontab -e;  crontab -l
来源：http://hz.quarkkingdee.top/gtlefsmpgr.html

[R67] 生成随机十六进制串
来源：http://hz.0kj1m.cn/gtnitvejud.html

openssl rand -hex 16
来源：http://hz.yvedp.cn/gtbgiapata.html

[R68] 计算文件校验值
来源：http://hz.birdmap.top/gtorxbftjr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangkeji.top/gtmjfpwfxr.html

[R69] 生成随机密码
来源：http://hz.jqgfzy.top/gtqnyjghrh.html

head -c 16 /dev/urandom | base64
来源：http://hz.tian-w.cn/gtuvvfecwm.html

[R70] 时间戳与互转
来源：http://hz.tian-w.cn/gtobwgryru.html

date +%s;  date -d @1700000000
来源：http://hz.yonumen.top/gteiwyywil.html

[R71] 日期格式化
来源：http://hz.xuanzx.com/gtmidbmego.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hongshengwenyu.top/gtfrluifee.html

[R72] 等待端口就绪
来源：http://hz.guowangkeji.top/gtdavjnziw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xziqi.cn/gtgjbpzanu.html

[R73] 分割大日志
来源：http://hz.guowangkeji.top/gtrihmvdiq.html

split -l 1000 big.log part_
来源：http://hz.yj20258888.top/gtgdtdvefo.html

[R74] 批量重命名
来源：http://hz.haohaochexian.top/gtjunamxde.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sufxvd.cn/gtvkzpvqap.html

[R75] 导出环境变量
来源：http://hz.shanyushiyangtech.top/gtowscygtx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ppjwa.cn/gtavbiyofv.html

[R76] 使用临时文件
来源：http://hz.gzhubu.top/gtxcfrifrr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinyuanbaomall.cn/gtgfyatlqz.html

[R77] 读取用户输入
来源：http://hz.andypj.xyz/gtshttiywa.html

read -rp "请输入: " ans
来源：http://hz.yongpay.top/gtkdpxpndv.html

[R78] 交互式菜单
来源：http://hz.cashguo.top/gtmyrvndrl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shanyushiyangtech.top/gtdkeowcwk.html

[R79] 解析命令行选项
来源：http://hz.chenzaomai.com/gtgioisbzy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tianlin.xyz/gtrddtbhsv.html

[R80] 查看脚本执行耗时
来源：http://hz.zhongyouzk.top/gtewnxmcci.html

time ./run.sh
来源：http://hz.guannengcc.top/gtbbcohfiq.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gttxggyzfp.html

S. C / C++ 专题
来源：http://hz.jinqigufen.top/gtstagewto.html

================================================================================
来源：http://hz.hywenlv.cn/gtpfkhbcuh.html

[S01] C：Hello World
来源：http://hz.gogol.net.cn/gtbueuwrgc.html

#include <stdio.h>
来源：http://hz.bjfxy.top/gtnvsvgdtg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.meibo888.top/gtanjanqcn.html

[S02] C：变量与格式化输出
来源：http://hz.haohaochexian.top/gtelkdlcbp.html

int a = 10; printf("%d\n", a);
来源：http://hz.haohaochexian.top/gtncmpwkoa.html

[S03] C：读入整数
来源：http://hz.yuxming.cn/gthcnolvrz.html

int x; scanf("%d", &x);
来源：http://hz.yanxiufei.cn/gtqhbhhwsc.html

[S04] C：字符串复制
来源：http://hz.hysaishi.cn/gtmxsuhpjw.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.svipenyu.cn/gtmhqfysgg.html

[S05] C：字符串长度
来源：http://hz.shanyushiyangkeji.top/gttkegpayh.html

strlen(s)
来源：http://hz.sufxvd.cn/gtvdjegmwx.html

[S06] C：字符串比较
来源：http://hz.yonumen.top/gtlfvozsmo.html

strcmp(a, b) == 0
来源：http://hz.hongshengwenyu.top/gtdrrhmtnu.html

[S07] C：数组遍历求和
来源：http://hz.cashguo.top/gtnbevsvxh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xuanzx.com/gtanxtpapw.html

[S08] C：动态内存分配与释放
来源：http://hz.yangfankeji.com/gthytktdcz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.daria6918.cn/gtdeqgmngn.html

[S09] C：结构体定义与初始化
来源：http://hz.yj202588.top/gthecqzrbg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tanke756.top/gtzdxbbvig.html

[S10] C：指针与解引用
来源：http://hz.cucudq.cn/gtflrqjxqv.html

int *p = &a;  *p = 5;
来源：http://hz.yuxming.cn/gtvdcuyyzh.html

[S11] C：逐行读文件
来源：http://hz.fzhhl.top/gtfljshnod.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhengqikj.top/gtvcujjwem.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhijiandao.cn/gtzjifbjoz.html

fclose(f);
来源：http://hz.gogol.net.cn/gtmtcummzj.html

[S12] C：写文件
来源：http://hz.havefunace.top/gtbrynflwd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yongpay.top/gtowfztegg.html

[S13] C：宏定义
来源：http://hz.xuanzx.com/gtveeottqe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yonumen.top/gtnyjdyuin.html

[S14] C：枚举
来源：http://hz.yuxming.cn/gtijdsvpve.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cheryme.top/gthhederju.html

[S15] C：类型转换
来源：http://hz.jyoumei.cn/gtnhfhnaav.html

(double) a / b
来源：http://hz.c1oappe.top/gtsifvwmkb.html

[S16] C：位操作置位
来源：http://hz.guowangkeji.top/gtgfjdqfph.html

x |= (1 << 3);
来源：http://hz.chenzaomai.com/gtqssonwnk.html

[S17] C：安全拼接字符串
来源：http://hz.chenlongwang.top/gtkesbfnpc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gaohongyu789.top/gtfgdwlqhd.html

[S18] C：命令行参数
来源：http://hz.yj20258.top/gtnoudfypw.html

int main(int argc, char **argv)
来源：http://hz.jianghu66.top/gtmdtzsdtr.html

[S19] C：快速排序
来源：http://hz.chenzaomai.com/gtgqmochin.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hywenlv.cn/gtqtgqofwl.html

[S20] C：二分查找
来源：http://hz.xinyue.icu/gtnipkhqoa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nanxuanxn.top/gtfcszqosx.html

[S21] C：字符类别判断
来源：http://hz.sysykeji.top/gtkcoydyyh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yueranfly.top/gtvxrovofe.html

[S22] C：字符串转数字
来源：http://hz.nanxuanxn.top/gtwmagrlsu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sxryk.cn/gtylfnqalb.html

[S23] C：随机数
来源：http://hz.zhongyouzk.top/gtdpghgiqd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yonumen.top/gtsghemcei.html

[S24] C：获取本地时间
来源：http://hz.feifeiyinyue.top/gtlnptwasw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jiagoushi.top/gtrtzmjvmq.html

[S25] C：内存拷贝
来源：http://hz.gotoacloud.top/gtjdemcijc.html

memcpy(dst, src, n);
来源：http://hz.ybcxt.top/gttqgcnryq.html

[S26] C：内存清零
来源：http://hz.shuidangran.top/gtdpnpetkt.html

memset(a, 0, sizeof a);
来源：http://hz.yj20258888.top/gtmnrcujzp.html

[S27] C：定义常量
来源：http://hz.jyoumei.cn/gtigckkqti.html

const double PI = 3.14159;
来源：http://hz.cqqwz.cn/gthnxjnacb.html

[S28] C：静态变量
来源：http://hz.zhoulong.xyz/gtyxfyuprn.html

static int counter = 0;
来源：http://hz.jinyuanbaomall.cn/gtlvqkqgmx.html

[S29] C：变参函数
来源：http://hz.tanke756.top/gtieuudwpc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxuanxn.top/gtnjkxppme.html

[S30] C：头文件保护
来源：http://hz.ppjwa.cn/gtnuqtdhvc.html

#ifndef X_H
来源：http://hz.fengsongda.top/gttaanoyne.html

#define X_H
来源：http://hz.ppjwa.cn/gtwcfoauea.html

#endif
来源：http://hz.meibo888.top/gtnzimvnqy.html

[S31] C++：Hello World
来源：http://hz.gogol.net.cn/gtsgydylmr.html

#include <iostream>
来源：http://hz.andypj.xyz/gtgoplegdy.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hnxiangtu.top/gtjghvpwgg.html

[S32] C++：字符串
来源：http://hz.meibo888.top/gtfonwjibb.html

std::string s = "hi";  s += "!";
来源：http://hz.hfpthk.cn/gtyqeeikul.html

[S33] C++：vector 增删
来源：http://hz.yangfankeji.com/gtjurqqlar.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ydjk.org.cn/gtxzdqxfrl.html

[S34] C++：遍历 vector
来源：http://hz.zhongyouzk.top/gtdzvmtfcn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fzhhl.top/gtnqhpvuzl.html

[S35] C++：map
来源：http://hz.guannengcc.top/gtdrlsgjut.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinghuilouyu.cn/gtjbbjqply.html

[S36] C++：unordered_map
来源：http://hz.9152youxi.cn/gtpzgdrpcq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ybcxt.top/gtyasyatcz.html

[S37] C++：set
来源：http://hz.tian-w.cn/gtpagdwflx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.tanke756.top/gtdzicevmo.html

[S38] C++：排序
来源：http://hz.yangfankeji.com/gtigxxmphl.html

std::sort(v.begin(), v.end());
来源：http://hz.9152youxi.cn/gtxqlnyfhd.html

[S39] C++：自定义比较器排序
来源：http://hz.gotoacloud.top/gtejmmyomk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nwbrower.top/gtuuwqjjru.html

[S40] C++：查找元素
来源：http://hz.hnxiangtu.top/gtazrpkaua.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jqgfzy.top/gthafrmtgn.html

[S41] C++：类与构造函数
来源：http://hz.yj20258.top/gtlzinckkf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cdnleiting.top/gtoawmdroc.html

[S42] C++：继承与虚函数
来源：http://hz.jyoumei.cn/gtvavtsbjv.html

class B : public Base { public: void f() override {} };
来源：http://hz.havefunace.top/gtpowbuuvd.html

[S43] C++：智能指针
来源：http://hz.yangfankeji.com/gtlqdupjrl.html

auto p = std::make_unique<int>(5);
来源：http://hz.meibo888.top/gtzhjfmwvz.html

[S44] C++：引用传参
来源：http://hz.xylfe.cn/gtdtvsrzyv.html

void inc(int &x) { ++x; }
来源：http://hz.ivvv.top/gtavgpkssl.html

[S45] C++：lambda
来源：http://hz.redwolf501.top/gtdnzfqwad.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.chenjidiqi.icu/gtgtrvkubd.html

[S46] C++：函数模板
来源：http://hz.gogol.net.cn/gtxtxufzpv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.birdmap.top/gtdgvqpupf.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhaomingkeji.xyz/gtgkhhaxrv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xziqi.cn/gtjhorjxcz.html

[S48] C++：逐行读文件
来源：http://hz.cqqwz.cn/gtxanjuyck.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.9152youxi.cn/gtlozbasgb.html

while (std::getline(in, line)) { }
来源：http://hz.andypj.xyz/gtadqxvqee.html

[S49] C++：写文件
来源：http://hz.mhx1999.top/gticmvgqsx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tian-w.cn/gtlngbxcnx.html

[S50] C++：格式化数字
来源：http://hz.jinqigfzy.top/gthzqnlrkg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xziqi.cn/gtkzvgjwdp.html

[S51] C++：显式类型转换
来源：http://hz.xuanzx.com/gtmvuzzsow.html

static_cast<double>(a) / b
来源：http://hz.jqgufenzy.top/gtagwpygfv.html

[S52] C++：const 与 noexcept
来源：http://hz.nanxuanxn.top/gtcqekohfx.html

int size() const noexcept { return n_; }
来源：http://hz.xylfe.cn/gtjioajnal.html

[S53] C++：移动语义
来源：http://hz.dashuyun.cn/gtwhhmpzdn.html

std::vector<int> w = std::move(v);
来源：http://hz.bjfxy.top/gtvrlvizwt.html

[S54] C++：异常处理
来源：http://hz.yangfankeji.com/gtapbsgxpp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinghuilouyu.cn/gtyybgvpeo.html

[S55] C++：结构化绑定
来源：http://hz.sweek.top/gtcnzbnaah.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gogol.net.cn/gtocsinzti.html

[S56] C++：optional
来源：http://hz.xingfuxueyuan.xyz/gtrwhygxrg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.aibaodan.cn/gtendwalow.html

[S57] C++：编译期常量
来源：http://hz.redwolf501.top/gtwowxvzbc.html

constexpr int N = 10;
来源：http://hz.nwbrower.top/gtfyvdckuf.html

[S58] C++：命名空间
来源：http://hz.xylfe.cn/gtpbvpmspx.html

namespace ns { int f() { return 1; } }
来源：http://hz.xinyue.icu/gtulyojfxt.html

[S59] C++：静态断言
来源：http://hz.gotoacloud.top/gthmhziwtp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jiagoushi.top/gteoluvgqh.html

[S60] C++：遍历并删除元素
来源：http://hz.xingfuxueyuan.xyz/gtpimoeovg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhongyouzk.top/gtnqnlfxna.html

================================================================================
来源：http://hz.snrcjt.cn/gtpycbjtpc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tian-w.cn/gtcppdelln.html

================================================================================
来源：http://hz.vqdsnc.cn/gtcymmdklr.html

[T01] Kotlin：Hello World
来源：http://hz.dianchejie.cn/gthjhscdxo.html

println("Hello")
来源：http://hz.yuanzhike.top/gtwwrjzgjx.html

[T02] Kotlin：变量
来源：http://hz.xuanzx.com/gtzzglmzpp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yonumen.top/gtkamhlfxi.html


<!-- 参考信息 -->