代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mbltysve.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3xzrmmwsr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3iqlmijzx.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hmwgprug.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3axbljkok.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vmnakfom.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3fkzydejq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vdgifknt.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3yrdkdfmh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3uawcnxoh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3smynhfkq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hdcljiil.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3fmgdgeia.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3yvhtcfdj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3hepiiojv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ufyfiuxx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3hhsumtgr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mwmwvmnl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3txpklxpa.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3jipkyuwf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3xkvpltkz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3puhqjjii.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ofwjmoog.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3pnnzdgns.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3btlwopxf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ofburpta.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3oxunfmrg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zoqcvoel.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ompghtqt.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vvijhacr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3worffpel.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3oyhfhfoi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qonvgdss.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3davprakr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpzeiidy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3zccdqwvf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ctayseyy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ubrjrkfi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bpwmuydm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3htivnuho.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3bmwckxxg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3jsxsjree.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3gsurjjgp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3lzwrslfh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3htfxlnng.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3dgwfkhwa.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3pgytkpof.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3icqbbaoa.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gmrgjxkc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3dupvjxym.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3grnnjshk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jdkpzejq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bkmqwctw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3rwytsufn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gxybyrkc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3xuielsls.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3vceroqca.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3yxfyvfyq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3exensksh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3auefygib.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3rccnwcry.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3rtsdyejv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ncxifhtz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3kvyzuusf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fmlilnuc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jnsamcxh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pboguwrt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3yrgejkzm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3fpazzsfl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3yuzevxmw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pioipsnv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3cszoulme.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3aytdfmtn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wdkfjmmy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3sywspqzf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3hgbyleft.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3rzivgtcn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3nojescix.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wcbqazlh.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3dtdpxryk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3eohxphci.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pjfyrphe.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3wxibaxbp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3puavimai.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xegzhevw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xworfkif.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3sbbhdmzl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3szejlves.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3wgebxjwo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hkvwxawg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3vvmowqua.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3uifkvhzf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3njzdutwn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3lzkzepgp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3hgxpmfsb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3alfmnhjx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3naxfevik.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3pnikhssj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3scftqglv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ocgeiyah.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3hglxscjy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3bhlbiaox.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3joougwie.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3xuqjpclx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3kykrigjf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3wtpdqoju.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3rerjbhpb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3pvvkwohq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3yefeszyu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ilokmqwy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qlfnlwvi.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qmnqzqct.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wfcylsiq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3cxrijgwl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cpfzztcc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3syhnlptf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3tjavyilu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lxeynkmm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vnkuceej.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ryljnoze.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3gwsrvuee.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qpykutil.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tdopajak.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3qhocsxwl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3viljhgil.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3hgvvsazc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3egtniltb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3qdjuuecq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3fqmebvgt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3llepmhvc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3tummqils.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rjmzdcdc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lugakjjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tayqmmzk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pxgrmetz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3bgiobdkp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3bypzlulc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3bhcfesqk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3bokvcdjy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mnakyfri.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wurzralb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ifntowsi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3grvyknkm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zgrnnszd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjgjbmgf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vpmrdlsf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3hultlpfd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3albighwl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gtyqlixw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3iagywowk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3wlahyxxw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3cawpykty.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ezkwnuco.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qpwvlyqb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3nosuwxsw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nqyufkbi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3nseudxmq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bplzlxgr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vvxlptas.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3bmfxjfko.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3niazyetu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3pmbodphy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3zdpdxmsj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3hcoociag.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jthkjtkc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3gwspsixq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3xljmzhhi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cnnbukwv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dyvwquse.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3flmklkki.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3rwgqvpln.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3riaenbyi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dthakbay.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3axcgvcym.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pbtuozdf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3njgpvsuk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rtpecytb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3gwdmabsl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3dmqcmtij.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rxmjtvyo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3odkjufaj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3lxjvazzy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3bczrppct.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3nnvhucmj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ygdkylkk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jzvuuwlc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3tflvzbaq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3cthjtlpg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3jjfpujwp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3chlebijd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uguyykrz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3pdlqgkre.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3yfifcpyi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vbnadgld.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3xcekprsr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ccbvgmyr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wmmrfere.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ugqqntvj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3glcstioa.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vufmezhi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3zilyteuj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hixfiiru.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kukuuyok.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3atteezsv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3nytdwaew.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fkaysgdk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3peiqtown.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hvfekdbn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3frxkuwqf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ijapcuku.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3raovlosc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kmaidzbz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xiccezcc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eyanuvyx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ortvqjzg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hmajnjsj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3igxllgfq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ogxdghro.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3zcdfasbk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fyawidvz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3icgolaxm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3owamjqll.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3uqyozski.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3xtpboplq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3eiooqsxu.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3oipetlql.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3cteeucjn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3owjxolsp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3sjaquybm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3hdpwzkyx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3thequhde.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3tinbnokw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3edztzyrj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3kriupiew.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iuxxmepe.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3uupweshm.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3zzsermha.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3tntyopul.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3buodiixn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3iviaaehn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wzccbxjx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3kkolaaaw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ivqmyakj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ghfxdsdm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfddlxpw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vrbbalqx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3stsyjqbv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3zonrnvyb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3fijgdfhn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3velzcwpy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yqtqeaul.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3parlhfiy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzveoiqb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nfvlwpri.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3eynitzjn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zdzeogcr.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hyzlkgho.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3rinkmuwm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3jtwjvjdk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3lskizbgn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3snzvkezt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3srwskinx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3webauqij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jrvkczky.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cbbyagbk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mlarlfif.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3uwrvfmmc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3tvweakzf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3qrvzwprp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lbjmvwlp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3qbvgcgsk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3tcnvwllx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ufyhwgxa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3hcjpnrdq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xxkgimmb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gomzepzh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ftucifss.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3gpdrrodz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3togaxwmw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3stgbslri.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ppxrxiyb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3xabddwxm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jghwsrkl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3nppwlpxn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3sgkraezs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3xqdypqfe.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3zspsdlbd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ecntvbli.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xhvjhqlj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gvqonhur.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3buvugskj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mfjesatm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3koxzmlqv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3fxkzydco.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mfsoacos.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cubnsvzo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qbcxfifk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3oxhvgpmq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bvzswfsy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3mlwuejyh.html


<!-- 参考信息 -->