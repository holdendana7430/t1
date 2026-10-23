代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3yhkutndr.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3deoyjjco.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3unhzohru.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3korszdgl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ylfzbixs.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3wdukbplx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3jvjdrvur.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3zqwrpxua.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fwukzgmc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3dhprhhwz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3rttuynzn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3mnivnkkh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3muhrtksh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3xfbgppfo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ujqbgxnp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3yscbiwre.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3epxbmqri.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3eazafqyk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3bagvwnyo.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3iaxhkesc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3yapnoeyt.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3qprntsxm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3agqsutsa.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3cxrsizlf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vowfssyh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3djobcdcn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cuuvnheb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3gnrxrtns.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3hsresoha.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3qsnjvogg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pnskqzby.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3tifefhpr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3boyedrji.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3oejrdgik.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3idopapwp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3imbcncbg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3httxyssj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3bwotyhyf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hokkvgzi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3afavmxal.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rpzlisvk.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3eycnicqt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3rkpoxnhf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3elrsxosp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3jhdjaepr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3qdpzjisp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3drcbwcyn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fkixsxeo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3apjkthmx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rszgplpg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3wekzouea.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3uexyoyof.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3gtskjwer.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3bthckyqd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3kmlzzdzu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3stslcduj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3bwijyetn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3vfjjyrvv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3hqgmupev.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3emlmhabt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ydfydjgq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3csenxlhw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3arkfcvyp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3pigvfdow.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3jwmyckvb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3tlhpfgvz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3rnnzpmok.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3vewxlyqd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3snalcbdl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3rmtethyq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3nbpmsqrq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nbupygdp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3qwvrzonc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rvrlkght.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yvgttnvl.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3mpljtgld.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3iiuwigmy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3aarolarz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3almwetot.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hofzhcdk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3pnixugoy.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3fvmrpvvd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3yihqzgbw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3zozkrbaj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3cbmkubux.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3fsoxciiq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3cqdajphc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3vbrhksol.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3qvxjpllr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3apvofuxp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3pbsaiici.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebeecmxh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kfuikodt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztabgqrf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ghzeywhw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3shgprcrv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3alldmyfg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qmirqygz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3nuvumuwj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3knreyftg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3omzxmnhg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wxthbiyn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3imlbjmup.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3haawafzg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aklqlzlq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xpuvbtuk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ynerdbqv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3kylemmtt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3wqdohyqc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3amzkmhhp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ghgsxups.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3xjcqvkrj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3rsrjsvpn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3rbsdqpkb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ygdiwacx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tqqlbobf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3oiimhfll.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nlfofogn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gpqewgih.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3okikkjcj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ezagkxyv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ipeuwlqy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3bupbdvja.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dsyouhyr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3aigmgvtq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3pvubykpz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3tyisgtvb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3bffmxpve.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nkwewblz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pdkegkav.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3cxolshok.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3explqwuq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3praiikln.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hytxgpwt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ebdwkmyj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3kyhiwbhq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3huexudxo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3imampepq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3cxqhaezq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wllijmlm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3dnwynwel.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3peyiqzht.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3mbcpgrcl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3txmjtcya.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ljnpytxb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ouihpmbd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3jgpukble.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3qkvgvulv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3jxrhtnoq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3oowjoltz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3anlumihl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3lldbqtze.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3finmmsnk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ydpzlped.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ljshnaql.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3bjivybaf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3salpanot.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lvglcgwh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3pjmgrydh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nffwdlbd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3lhimkqqw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxhnemtq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3fpzhnjyz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3yoizcaor.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3rhcfihzn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3pkyyyzvl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qpipqsfd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rklmbozt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3nfzxwkzq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3grpqrudi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3jwiuxufg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ryvamaxa.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3gtxqkfnu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3gnxocikn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3pdxexopq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3symckicr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3habcncbr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3mxovjxsz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3mpbpsrxi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qppxgjyy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3yqucieht.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3kcsebrbz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3rccvveox.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3jbwgdugt.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3nsnizczo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kahncwmy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3hkwuzkqr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wadkdeoz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3jfhmwagu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3fazrhzmb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3yajqsvma.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zofhwskc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3djfrkeau.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3potrephx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bpsykjbp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3mjpzyuqi.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hcutnkgt.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rqbphhgr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3yxthmacc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3okyzrpjt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3epvlaqjf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3taejgluv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3obrukrdi.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gzbzcuqb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3kexlwzoq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3lbadhyic.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xcccjsnx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3maokzlfw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qosgnqie.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3jbxypvgx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wkymhmbj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3cidygfwz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3omqupsyt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3vopcsort.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3welnnnps.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fsaagwxh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3eroajymn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3bhirwhrr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3dztvuidk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3tpcwtwnm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xonnkiqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phsyklfw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dxnazqqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nazlfqar.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xzubizls.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bazxuees.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rhuloxeg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3myhznsmw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jtpyrzbp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ayvuxppx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3szmjmzid.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ctqrwvsx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3spmrqexf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3lrrpubnl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dmzncatq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yyucoqab.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ymscfsat.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3jdxchfyj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hkciahcu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3yocywoui.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3zakeetxy.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3dmifkmkx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3pnnokmsz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3nhprvblq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3znnnypns.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3dbngmrme.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3lgaznekc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3woohycju.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zurecsri.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3dhpuaist.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3sltekevy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3thxamwpi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3esnlwfdj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3lotqlbmc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ymeawipd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wqdbefny.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3mldqanif.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3vcjfrpur.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rtilpobg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3dzsqlcel.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ychfnjym.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3mrxkgqgw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3gmaywylh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kkpqcwdp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xooabcet.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3fjezuryz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qunoanvs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ojixkfhd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3kpsizzbk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3iwqikcmi.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3acwfsjri.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xinvytmb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3nagvvlku.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3unbzpxxv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vermhjhz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rkfxdpya.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3eibfpygz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3jldzpoxs.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mgopfnqi.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3uwdioxlv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3jkcjuxrr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3lmbsblpf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3kdeturbr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3qgdsnqkm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lsydyias.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cmqmtbij.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3geakvhyw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fhmgphkq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vkrlssea.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3mpgmaods.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qrycyczf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3uwqybnqh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vqqvuixv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kzqfblhl.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pbnvtuzl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3mxpfswed.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qcwimkcv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3pjnxsbro.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3mgquakie.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ekexsspd.html


<!-- 参考信息 -->