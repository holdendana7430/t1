代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zsqwttit.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3iwsklqgw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pgthutce.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3vxmioegi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bnlacpae.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ezkfzben.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3avexenpb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ropleyfq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pcflsier.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3kutxkplb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3doqxcwmw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3idevdxvr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3mpnmrrmi.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nghyfkkb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3mjzpiugk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ophxijlp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3neblgnmf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ijirvany.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rgixtcqv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ecvibpfw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3gutumhyd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3kmmvkapm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3vlfczqda.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3uihqusxk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fnfvdxim.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3vfylncrc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3wfjgqqbn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3smvmaygp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nplisyog.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kadfpvkx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3eyxjfroz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qcxpbykt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3cgpkkiri.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3zwewmqfc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3femjgwem.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ycjqqdgm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3gjeahzfl.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3muxaqpqs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hckowhhi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3iiscispc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3oixfsorx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3mmdwoned.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3vausvufv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3uhvrceyx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ntipibuv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3cyqjebnv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3qtexokfv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3hfhybayl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lyugteoj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bavfrcjr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3kdivzajp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ycdjsrmr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dnsxlpbr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3pdvwoced.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ergxfuan.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qdcvoitz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3tzirgxex.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3clvgaypl.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3cjamwhib.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3yvmcplmo.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3pjjjwtbq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3obimyibo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qmkfkaqh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3xigibswc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rktfipnc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3avtlklag.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jodhcppz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3elvjofdb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3pagaapge.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3bnhlcazh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rzyyxsth.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3iupfnivr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3gefxyqlo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ombrenmt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3eievnwgw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3iwdhffrm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ikpzekcg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3idoforws.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bvxyjpmb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3kjqrtftx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3dapybjom.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3llrpiltt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3plbudnyi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3pmzsrvez.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ngicrjaa.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ieqwuzmr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3gtjszdmj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3izgglwpb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3szscbuat.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ottfgbfl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3bahkauls.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3dgnuezdq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3frcgyhet.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3xlefumba.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tywannck.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3lqoulpuu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3suixsiij.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mwfywlix.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3mrgqmqof.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3aeurmtxt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3dpzccxpf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wmzsfwhu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3klxnfznw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3cepwcted.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3juqhgoru.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3efypuljd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ccihmqvq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3oqsmrtkm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3sacedxze.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3bwownpmp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ywzwzgtk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qaflcnhb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3jlotcspl.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3pkikzipr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fklrauhw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3llldgyjo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3nnuyctga.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3fufeymxy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3nfyfsrnq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3aurnjoxo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3puiifawf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3igiqyfxt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nxymkpnr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3lyzawfea.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3zrmkgqdm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ijpeqabb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hcsyxmxl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tgqmuglh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ptnkwlvp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mqbwuleq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3hxaxvtmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzjrskpm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xxchuxxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwnoxpwe.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hrcourpi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3xilpirte.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3szulfbgp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3bgzxkpdj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3twqtpmud.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ehlapnal.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3dxdvruko.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3fpfuqmwp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3euhwitpo.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bxwwnxem.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gbdlezcv.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xtfsvfyh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3frzzlmns.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3qfqdjpup.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3osxaimzf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qydxxnau.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3kpavngtj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3gojezekd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3iewkfjrx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ameabamc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rzfawjdv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fudktshw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3projcdik.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pbjzkbwy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zyismnow.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3oxearkxt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3geeasqfn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3eshtnzct.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fdfwftuu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3wqqqrczp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ygpamtyo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3wmaqhkgc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3qhcyxgiz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3oveeyzpm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3fyabfcsz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tcrdguys.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3fiummand.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lpfabdcu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3zimdtids.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3vkgwlthm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oqlocbgh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3fstamjdd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wikwwcbg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3viocnnkx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3bgrigeib.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kuwrvjwr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3cjzkpcbr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3eysczsvm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vbefwhyx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3aatbghpu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3cthhkfmt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3egyqrvql.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3fdsetvil.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3uvcgdcwl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3gwxhrmqz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3jrwfabmu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ytxoovpt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3pspozmlk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ycldxadh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3myvigyit.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ghdgglsr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ncdvboea.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xtjwnaut.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wdqvbgov.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jhzjifzf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vogtilck.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3bvzmegpe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3cpepftix.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3qoeminai.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3pnxndkpj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3gnkixgqc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3nbcsqahc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ymdrhhra.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3jvcrtyfq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3rrzupklp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3awplrvob.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3mhctfnop.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3haxupvwz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vwbliftm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nnzbolyd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mhkfvkpc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wgexhnar.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3gcykcfsz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ewqsvwys.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3gigecprr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3cvrvalug.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ovflkpkm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3odqghwuw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ypjwzamr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3uihdxvpt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3eewtguin.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qgujhtrl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3mcbgbzgm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffyjxabe.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ciidkhtk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3dgcfpscc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3hayeghsp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfsjnwib.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3unofavpo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3rnzmmazj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jcolifbj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3tlzfuqiu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3szzscgdk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3usnquoiu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lxekqbdt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3xaruxcpp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pfwzemgi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qpzzirpx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3olglxgsi.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3pmmzvray.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmxwrhuh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ahbaotuz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3tyzrhmdo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gbglntsh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bnmevfnt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3egyrnnac.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vpbgddmr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3qcxdoatr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ahxfwmuh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3dpfwrmpu.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3buiejhdh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3srcxiuqu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xvdcdqux.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3taemcafp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3mtqpyexh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kkezgjol.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3szsbnlty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aaidlrpr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3fanvfhqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ptwpbxvo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nrrkqsfz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jekadcek.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mbrwheih.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zqfmpxjz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3hrohrgib.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rwebgbta.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3avrgpmso.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3nterbnvo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hrlimzvy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3jdsgqouh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yvauzhkg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3loltbbub.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3laezvtyw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jcgeybaj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3woivqxzv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3abfbuayi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3uwbncrgk.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3fwgfcirk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3kiqhtskp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wfhwutkj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3fylzgifw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3gfbnjvai.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3odyldfjx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ouujcobk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3tqvfgdpe.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3fzokrpzk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3lubjmanu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xpdwsfmp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3sxqqfkha.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3cqzhvccv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nxrsorpc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bvysdxfv.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vircesus.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nbbrzrdk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bdbfmdyi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3wphahnge.html


<!-- 参考信息 -->