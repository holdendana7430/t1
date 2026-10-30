代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gqwprdhjw.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gsotoirdu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/glrprdkgo.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gnnxkzvad.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gelgbnlkt.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gtceosujl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gkcwwvyee.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gilecfutl.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gyujxsszn.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gfejfdfbd.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gentnzffj.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gskzjcazw.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/guesxkegv.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gyooenszu.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gdpwwwgjh.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gypqcljoo.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/ghlxdlmou.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gqebuzlqe.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gastrzaik.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gmtrypjpg.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gmnoziwzn.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gtqzyhnwk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gknssgrqn.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gpremciww.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gkakrhgrf.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gdphxdpuz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gfvwsehzp.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gdwlvyuyq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gbhvtdaco.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gjatpfobs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gqalopbes.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/grzlyevui.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gtegjxmdg.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gfhbricya.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gpzcbmsqv.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gtjlkexog.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gurnenzxv.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gaanlfpwz.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gknhxpytp.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/ggwunbumv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gmlfaeqnq.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/ghwcrcwli.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gltsfvzte.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gzdgfaspr.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gmlfcotmj.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gejssguop.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gxoslwqle.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gmtckzocv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gdygoldek.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gioltxewu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gtuoztgij.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gdkwzdopk.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gtgwvfiqg.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/guodxtxjo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gihwehzyz.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gbtoymujh.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gvequmjlp.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/goadepjoa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gbgiojvqm.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gfbqkyhfc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gscwtrbbz.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gsxqtrqkg.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gdjtxhyov.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gwvebkcsr.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gjsnqrwqw.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gglfqwroa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gfqpofnlh.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gxextxlmt.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/geznbmtcw.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gojdblbqy.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/ggfctxods.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gntoigmuy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gbgpyphnz.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gzsgdighe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gvvjnbozk.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gxbawmxjp.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/grjwsrmbf.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gxcgglark.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gktcztafm.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gfyfqjoac.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gfbwjdcpe.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gvjwxqzth.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/guzaknpep.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/glexvlbfm.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gwovevujo.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gqavuhfyx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gwnmvunrt.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gostycase.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/ggbvloqfd.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gmqpkvsut.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gfwsqtkjr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggkeazheo.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/ghcumlnwy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyiqwdivb.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gpizcdzmv.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gghghfxer.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gxbmiieka.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gytlzulox.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gzqcorwpw.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gmhdwaubc.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gwfkwrdjq.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/glbbnwrxu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gnudvmqcm.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gluogjkdd.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/geyzubojw.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/ghakmqsbh.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gkbtiwoit.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gynmjljjb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/guaxpzbau.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gftlifcgz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gyqnnhsxl.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gepynavup.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gqqylhkka.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gwlgedqho.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gtqqibwvx.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gfeldofcd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/grsmxiybk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gabhhmfuq.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gfhhqsezb.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gghbpjbcy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/grrspaqpb.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gelgxghuo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gsiqlryam.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gsbguzcrc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gfznmwfbm.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gaeaykwuu.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gojtzoryo.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gsadoybov.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gofdmotfn.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gxllqcmro.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/goyyxomqo.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gongtfukj.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gtlnckjha.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gnjmvimva.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gxkjvtvrx.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gcsbpdsmi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gvbqbraau.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gwomwfsml.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gublopbcz.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gormbcmor.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gvwlthzjg.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gmichxcti.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gkrksjxxd.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gcdgkfjvq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gyceugbcj.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gykybdyjs.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gynyujxvw.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/grhxyraco.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gfhfwbkbq.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gyvltmheb.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gvupfysia.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gvsdnujjh.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/grjnijumx.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gnaromkeq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gasgdyoux.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gjshxnnfw.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gcawnyggs.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gghovoisy.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gzkypefck.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gclgcnelj.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gzcxvgtit.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/glyrnrevo.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/goejpykie.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gdilduddc.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gmssgcxmn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gvdveheez.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gsqvtnkdj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gphxvnaxz.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gaqfbjmde.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gdapsbomv.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/ghibpodiy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gelgxmgog.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gldykifpb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gktsztdsy.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gyfgoahjx.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/ghtcryhqm.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gotmhcbjj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gjubokepy.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gcwnehynj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/guzpueims.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gutjtmzmb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gdrnbhswl.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gnomeciok.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gmlrgjpml.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gimuyijdm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gnlegtjho.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gyrbcvydg.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gkezfxath.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gpthsdbku.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/ghqwwlede.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gglxjrmpz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/getthszyg.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gjdfeirbd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gwttmtrvw.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gahofisuh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gsofmpptd.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gxdyehwlb.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gzzigervb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gajiqvnwp.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/ggsydvhyd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gulrsamay.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gmkaleike.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gnkwukrdf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/ghjndelfu.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/grgvjvlqg.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gucjpshkp.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gnawbhaeo.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gddilxabk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gxpkxivjd.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gzxbujjsk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gmxumxqal.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gswrpykyv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gwlcipvpg.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gcgksayiv.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gqfohkjde.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gkzxhhvrm.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gjewnuxdo.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/glrvheixa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gltazfpmc.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gfqcsiaub.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gtwdsimsf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gysbwxcjy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gbpybfakv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grrdmffws.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gwplzlqlf.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/grjuqlwoe.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gaeqwpzfy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gsmnwqvna.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gfceltsxe.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/goksdmqeo.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/ghmjjlieo.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/ghmcnstcc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gyrfkcnra.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gqqdfnhip.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gmfdkuciv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gyuvxzykp.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gmkggtrax.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gjvmrqufv.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gxfyldvgd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gzurlqygr.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gytprqqxj.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gvrbukqjx.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/ghplgweyj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gndwmawca.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gwuxriqjp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/goymgauba.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gwcwxhtnt.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gmxikamso.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/guosiglov.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gximhbplw.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gqjsjoguc.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/glsgkiewi.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gjvsgjyzi.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gngxkuztd.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gkjokdgiw.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gcrngdjtr.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gqzwatwmk.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gwbvbnnwl.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gpmjshsxi.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/guwgcxyzi.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gpwguttxi.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gyusktkyg.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gpceiriyq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gruhpifvv.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gbswpenet.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gehuvymmd.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gypgjkppp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gffqzflgl.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gvzmodtkh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/geyiuwcxn.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gtycrkpsu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gaxhhnmkz.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/grgmysect.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gbcajbcay.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gomgzbijl.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gdglmtyyc.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gmxcvldoi.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gbblslitx.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gyjgbmrex.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/ggckkjexd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gjzwdgzlv.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gselktlaq.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/givzsccxy.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gskonafzu.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/ggcgrjpui.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gcgmavzgg.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gbzoanccy.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gnaatqieb.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/ghfzeongl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gpaiamfoo.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gamnecpfj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gwshmfqqr.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gucirejdv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gtqmbiavo.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gfgijqgse.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/ghbcbpjex.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gxcaazmcx.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gogfvuynl.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gkednxzvz.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gqfqsglcv.sHtML


<!-- 参考信息 -->