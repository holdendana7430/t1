代发 wailian999

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ejwxpbjv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jshxdclt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3kabnbbsc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tshzetes.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vbgpsfqy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3sabilujo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3lfkyqrzo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3tgdsnyqa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3oamfrakc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ndzraeoj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3bvslelty.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3wdjevdke.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3himjckpk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3zjthwxkx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3yaalhgvu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3taiynuke.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3gqtbzefy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3bduwvsmn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3tpeldsxn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3uldloguq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkkgwmjo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3neicivzf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdohmegj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3krietdar.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3nrdszewt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3mgeqxuxe.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kkiuedvc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cgenjrig.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3jzoaeihk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3mhtoyazg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3xgftquhi.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3gayezbxf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3fauhuzss.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3vpdodjuy.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3etmpccum.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3aqfhajov.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xpkcmfie.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3udqjlblp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3afitfcsw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3bjmrhnqm.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mycgonfs.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hciydyka.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ktfirtny.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3mrxpajuq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3epnbmxhh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3vozaljvo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ugxjqjol.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3dbiyitsv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ayxhhruo.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3iiwfjacg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3vwkuedfe.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3qowefykp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bfrcxvbd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vifgiilc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ftxnsdib.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3acnkbdyj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3bczbthaa.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3dnvlwygv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kzymsulq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3bvcwugyy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3uomqqfwv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mykomzhw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3sfuseliz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zuifyuxe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3txxbzpoc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xaflygut.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ulngrbzp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3htxnldwa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3gwomzicy.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3fwtjgggt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3acvgrspb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3cktjwefx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3gjxsgrff.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3iajyjaem.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3vguilajq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hcsacimr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3hvcrrjrk.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rtibojfu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3fzfrtput.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3csscpesc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3blkdmgxg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wqhbjnyh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qdhhxgzg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3rzfioeis.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3oukqlpiw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3fzytjvlq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3gblhwecc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3xenopbxt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3tobxahjj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3uigkxxsv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3egugjypv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3wkgxjzuw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3wpckohdy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3rvnplbdc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cephcumr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3qfsyxfxu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3hulzhqxy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3hhxqfwgp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3gyjcxbeb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yqwmfewp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3eesdvias.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ivxmqytp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zeftwzbm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3yzsxellb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3buizdcci.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dxhulhum.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ulnmnzte.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yborwyan.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3pkhkvqzh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3mbojewlx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nmhmmoqk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3btdwqgnv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3iqouwssb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3gjrxjcri.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ljbzztmg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3jzdindqc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ponuqcsx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3mbzlewya.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3acvypxcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwtfshdx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zkezrnjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqgbcnrx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lcfknidg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3zcxhfwwq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfefndsy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3yvrexjcq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3gllywaok.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3gbpsedqp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3dlroaywz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3tiulxoeo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3lxhqnqtu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jkwxxcuq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qmiqvtet.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3biokzfhh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3vcwgfhxc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3akiqjclv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3autgjhoa.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tydpacqa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3olmkaozq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3skanoplx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xsfmkjwd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3fkmndetq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ehvhktkd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gyinyxeh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ehjnilnz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ftnmflzr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3iwghljuk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3iirqzcyd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fttnyojl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3qqbpsoos.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3oefjgulx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zbhuptka.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3qnoapxoj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3aqiafjkr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3iabbunwl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cwbrcdos.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3jvsjhvux.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sawgohzr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3npkwhedf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3huuplibp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3yghbpltu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zwnqnpeh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jwpzfvxl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3dqyvmyrc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bvhtrkcf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3bloshzei.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3nvlcjzof.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zfrfvkjr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3dpjmpygp.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3cvbfsmbm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3eberprvd.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3iwzqdrou.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dqmwyucb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3muqiulta.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xknbbgxv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3cylybwnf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3cqrobzyq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3kbyduwut.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mnqqqdhl.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3fhmmrugs.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fyeqpqom.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3hclhgrcv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3pmosmyoj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3jonectsc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jognydua.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3wukqcaor.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3fxgubnja.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kuphamwn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ccckmjyz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3riswtcey.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3lxhjnsli.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ltqsrlgf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3spwhtcij.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3jbhyuqbh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3eulfbeod.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzblkmpd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3uhcvvzsb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3aoxvsmzx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tvakqjun.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hpzczeeq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3gwjkzwuq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ppheabwu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3qmjfeopb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qlnzrckx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3tagyemvy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lriuwzhd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ivxpblty.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3uxvqjuom.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3kfphwoct.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3rslbdxea.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3cahnnxta.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3yahxaciw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qunchine.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ghbzglmh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3rujkhvzv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3qrlsuxrc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xhlzkvyc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3gsgwseit.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3kswpkvhu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ubktuurs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3svnuazkt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkapsdqq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3styaqrbc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3cuizerfz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ustmdcng.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3jwyjceko.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ntfskids.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3enjeubtg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wuvlsdjl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jnkjzmni.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3crsjstei.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3wfecjzil.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3hvwitjgj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ozxibbit.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ooqbojnv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3oczlgntl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3luxwupsn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bwtxsfva.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iyqvxxzt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3yuaazzpl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ciaveinw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cxmqwlut.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3epvmotyy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3aiwkhjtr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3yvkqgjgh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3yoovulje.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3kwbbqlvq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cvxymljf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pzxrbvar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivoysknt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ndufzcvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aaxpadxw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jzskmqsn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nqulumqp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3psfrvhcd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3vucnjejf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3cyayhjkp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3sqdtdpgq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ruituogi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3pspwjksr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3dzceuffk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3wbshxvbc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3okhoxjpn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eyeowgsm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ucvgiozs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3oiitpoma.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ciavjuue.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bzpzysmp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mzqtlpjg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3jqybitqu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rjhqiuby.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3lfnmamhj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vigffjhe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3nelmdcbs.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3gqotnpwl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ybaagtsh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3axtavkfp.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3cboptvat.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xonxxqui.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cqafwuec.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3xvmegxfm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3agdpzfws.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jqrcocmn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rudnhjej.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3krqshmdb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3kbfqymch.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qqyuyaif.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3tvvpkgol.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ecgslqdb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3kxxktnlw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3yivhpwxz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3snfufxkx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fmjhtvve.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zujkhqwi.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3nvhvhamo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3abjkgoxs.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3jlhhzrpu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ovigalvl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lsyheggm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ylmfpgcv.html


<!-- 参考信息 -->