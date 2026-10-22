代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2tlzbjiqc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2okpcrndu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2kqaovzsm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2qrqpbpah.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2yzvifahw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2zducwovf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2eganaubv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gmbamkqt.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2rxkyweia.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2owfcvjxw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2actvcjon.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2iltjjjnk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ldmgnzob.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2dinwrned.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hipqxpvx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xchwriqh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cjgyeltn.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2nkafvjnx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vufdkkxv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2rkxfmsyp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2tfmmpnwd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2iieilapc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aodyxatf.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rspwjzeh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2fmhzktmh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2udxxzhbt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ubpjgtao.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2swaqnylv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2bpwmlfpw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zqcxhgpq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bpdcclrl.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vmiihjjj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2vungtwcf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2iiddasnz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2orfxrqzz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2lbjgjlwl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wjmhbpob.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rekildsb.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2mqszfueo.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2eaooaamy.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mdnqrsbe.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2tquoiith.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2uqcajpeo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gtwcafxv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ompijfzs.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2dicnnxck.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mijtskii.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2yxusozcx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2rjabhcee.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2khljvdvh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekjcwauf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2vlysrysu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2wrtlhsvk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2rxdcpupr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tewxvixq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qafpaaih.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2alnwfltx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2scuboscp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2llyrkhes.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2gnivlgbf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2lxvrevyq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2mukaexkt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2nvddvmfh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2eolwtocv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lddihxdp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2smptkxyl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2wnnfbmxa.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2rdlhllrj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tnanvcpv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2efndevdl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2rvbnxxui.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2bdjnnafu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2yjkwiaxx.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qbbmtbbo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gipwtelh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tpjpbmnp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2datdpzez.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ywlxvktw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2poehvvqr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2dtvaoznq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2saxginvn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ltfcolfo.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2sryzjqdr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2njgdefzy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2dweajswv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2nwbcxvjw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wpcklnca.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2qjikcpoz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2tiqpujht.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2nuarbjsv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2kidsnjbj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2kplufwyz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hdbbaqvu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2oeummhet.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2kwohyhxk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2lqrhisht.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2jonlkeru.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2vmqsrraj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ddsorkgo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2vqzilfhl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2dsgfdete.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tzdbodhk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2uyjjcaxo.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yedunajt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2jmkvgkic.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jfspwlxc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2trshutzj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2kwwxdgwo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xmzlsdcb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2hqvutfbr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2bznkhiio.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2adsshqgo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2zgiegfpm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ewhgaway.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ftbpnble.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2iuldmzpm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2afofakut.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2qouirlwx.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2slytvalk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2qxvxmmvp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2fiiqwgul.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2upvhybul.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uyrzjrhk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2jfsqaqne.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2dhtwhnes.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2yjsoimrq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2pxghmaty.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zvxnyser.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2lxmfeefo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2lixuooml.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2amilpzzr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2myocohxw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2mgomgxdd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2hpdbywsz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2frmwvine.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2eacokwbk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2iibcikkk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2rjxggyyo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2izynlmws.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2oetqsxwi.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2inbidfis.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2srgszayq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2knxguobd.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2kmsefrvd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2wfdgethu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2uvvfiosx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2lveojymw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulcwvtsf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fromwfqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exzsxsao.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yhjnltgo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2jzigvaae.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioyzyrrd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kxdrqjwx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2trnmdvec.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2xqckevew.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2glsvsjbn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2kaiultsi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2uxtwkrjz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ievhbbxx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2awyoanpx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gewyftur.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2enbsalil.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ahmvzijf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2tbwgwzdw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2czjksvgn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2dfmolvpw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2jsxztuij.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2cmgumnlc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2zoppirly.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2azqzgzka.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uhenlowx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2xypcotss.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ztewzwce.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zisexoha.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vledairp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bkqkwdou.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2uokpvxjp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2eejbynwl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2llewfwle.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2fdhbjvyw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2dinqtaye.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ibahnpal.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2wlowyosc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2payjqdop.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kizjjdzi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2wwyojwxy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2oogtstnv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ljrbnohj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jilfvlye.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2znrarwrh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vzscupwd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tvbcyfzq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qrapxxht.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2vcwzigqf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gephjjsb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2tqoroglr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2mifljdyy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2gjdrvyss.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2wdfeybej.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2xdztyljf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lkcyyjfl.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2arhenxyl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zwyqlgkg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2wgihjkmk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2sqhtobtd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tczpwliv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2bnvtftbx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2yujfegdk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hxvoiorn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2tdmnlxvt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2bxunpzwe.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ohqpkdgd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pgmfeevk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2yrmyensn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uqzwectv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ksfxiife.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2fqkfacwl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2qrjkqbzi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ajsfyggv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ougahlyu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2nlkiaxgs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2smcbtflb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zspoirze.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2zhyckrrm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2amtvzats.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2agowjrex.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tbjbgyei.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2nskdowld.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gjfvnwjk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2rktsrpfl.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2anwwktpz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2owhuerfy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2csqurtir.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2bjallqkg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2yutwzwka.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2syxgcxup.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jcbxwmem.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2pffialpg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bwinynog.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2gydavojd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xwzfrltc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2zbgcapbb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmqhybhl.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2npvyyqnz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2nkdmnawa.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2kyxayzgg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uealewmd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2vossqegm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmgwqptg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jdxkxhvp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2czxnyltg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2iszxxckq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jdzjcdcu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xqtafknl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2tnphakuh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nwjkteai.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wncrnxno.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2inugqwla.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2eeawajaf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpjvhlcs.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2myfdhsui.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2uhffdmxy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2bftedrgh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2csdsjrqo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wsauocwv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2dcvuqmzm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2cljfblof.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jagheytn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2fvlcneje.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2bxwtkrzp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ryxpzswn.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2bawxopej.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2jgclcgzl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2oowmvegm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zopfbdrw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2atlevveg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rneythpk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2pzfeouiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pojgxsep.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iagqbtvk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ecadeitw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lrozudor.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2izuaupwe.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2osmqavhz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xmfvmwjj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2lsmuxqqo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2cbczrmwx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2pphufhss.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2forzgwca.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hkcypilv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dnrcsrvt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qomgamvm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2feykdwgq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2cgsbxdpd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2osfljmav.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2haaxtjly.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2psxdfhlh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tpglajyh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2dsucbsvv.html


<!-- 参考信息 -->