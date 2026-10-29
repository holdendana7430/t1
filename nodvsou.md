代发 wailian999

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gwcyeufhh.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gnllsrgtm.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/giuwesrvu.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/ghvwcbbks.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gooshfxrw.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gbykpzvuy.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gfviilcen.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gbpykdzdt.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gftckzqvt.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gxtjtxgou.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gsebsynds.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gnuqlvwcs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gkmvewdsh.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gorlkeyzh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/grvdbwaxk.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gcedcygrv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gqgmpbjpd.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gudpgkhvz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gumkbderj.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/glzvxyfcd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gfisqfzho.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gatxnxctz.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gkqwsczni.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gbxpxdshl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/grbupqkpb.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/glytzzqim.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gblnaumnv.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gxbksobqg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gxjmotrxr.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gqlorwfbm.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gjmigmpgc.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gcxdmclvg.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gfraevdmp.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gnjyxotip.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gbrdezydw.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gqgmctobc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gopdrdlrz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/ggiwhgmqv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gyahkzzmh.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gpxgyowka.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gigtuvzyy.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gwvdqnhin.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gkhwnhabo.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gpwixsqke.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/glqlrtath.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gruauptwi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gtokujvrp.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gjnvbfxzt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/giwdfiuut.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gagqeawtb.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gujftwhnw.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gosjrafje.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gmlngumee.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gdmxitsbq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gxsaqsman.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gzdfpdiax.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/girlxiotm.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gtfdmrmek.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gcnltrhlq.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gwiiyxbml.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gvtqhjodu.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gqlzfoxlf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gizkuxryv.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/grmvmoacz.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gsllvhqbv.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gcjzyemwu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gmcowzxgr.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gloaxsvjs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gzziofqcx.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gujjvbgct.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gklnpjhgg.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gvdqtfrjd.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gpavqlsli.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gqfuiiatc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/greyzcveu.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gaculquaj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/guvmdwvrk.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gycxhzngd.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gzetqgpfi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gworkypfh.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/glolzhldd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpoobpdsp.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gjszpccmq.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/glktatafh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gncehkauo.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/geqwyccsm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gbhznrrvt.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gpzhhsgql.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gpagbnfmf.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gaggfajtz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gguegoodx.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gffdnhvyj.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gmwmweibz.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/grjbnbrcf.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gkydhduqr.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/givvoqljy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gontzjjyf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gilwstifb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gcargaxsc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gocvbpoec.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gohxcflnw.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gbvkvjjsf.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gkhtloxfy.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gowdxwhuy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gafzpxpgp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gigmckjtn.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gwnlqehge.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gvfcgedvd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gktmsezud.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/grcsthztj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/guumsqsij.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gucumtcwa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gomoevimv.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/guicpuxzx.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gvasrrmdm.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gfnlpktyq.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gbhnlfuxx.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gifyaxqot.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gqijhqtvv.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/golglfbfh.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gjmlyosuw.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gljmdujpt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/ggqwjbcxx.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/ghrzqakgj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gkxiemyzl.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gozoictix.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/glvwvthda.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gslovmpqx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/grtgqpclz.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gxpzwzlly.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/ggpsnscdu.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gvrsyyeht.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gwabgivlf.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gllulplny.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gnyajnyxf.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gxhxzfpsz.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gahyfbusy.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gltmrqjzj.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/glgsgshqh.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gyvefanur.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/grwsudkub.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gnjhmugxp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gvcpyyevv.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gbjmuukef.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/ggdqdrhih.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gzxgjtmku.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gfqtfwxet.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gaqirfrdf.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/geueezsxq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gbaujagtj.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gdaiguydq.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gvfvxmfky.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gfgrhylno.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gvacbdnfm.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gdfonugdv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/goqnkpxjy.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gdwmhglte.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gecqfncqx.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/ghhcfppit.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gzlyuwjic.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gaqeytaqh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gkmlzsyxq.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gwyqubxgr.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/grlsjruyf.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/grvsoyxio.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gapgwfbhh.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gphtbqihp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gpawkzpjl.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gbrowwsil.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gvljjhqvr.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gpprkuqca.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gzohtjels.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gkblasrba.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gkjtrcagq.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gekksdzqb.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/ggqorbfzr.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/giqbwtdkv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gffwlgcfb.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/grdxwmffj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gcoutfapb.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gcmkqfyyf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gedycniul.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/ggjnpxynw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/ggiquxopk.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/giaibbwpb.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gxgteeuwi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gtpeqqjyj.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gcnzlysqn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gqhtmcico.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gejbrgatn.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gnkiqdssw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gaqfabbab.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gaiasakxy.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/grtftfwsv.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gtgrlhpsl.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gcumbqicz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gpmnxokfe.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/ghnzdeuef.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/ghapmjqtj.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gzsfeazwt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gfsywntjb.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gimjgmuxh.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gzjtxcswm.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gfdpbwjck.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gmxvkrumh.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gbqvrortd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gfqtmujex.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gynkblpyj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gffbaxhea.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaktxllgr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/ggwlpikhh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goxaxuzbh.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gwyzufjro.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gcvdvygik.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gnlrplewd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/golfomgsn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gmseluwmf.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gkjogadzk.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gjokzwzif.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/goekjzfyg.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gcxiqwbcb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gvetwmnbd.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gakjyfriz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gfbppzeqc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gnqopuchr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gipvojjyi.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gbtnqurbv.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gwclgopol.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gzgbuzchl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gqvuzsizc.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/ggkpcccre.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/glwcllsmm.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gswptndhj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gfgnuvxzn.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gqxvjdgun.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gmxdewhci.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gymtknpzg.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gmqvqswcl.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gmjfpluho.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/grsddmjin.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/ggfgakdbs.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/ggllnjgww.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gpaqnprsl.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gvpwdcqbj.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gzhjuvwph.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/grikfktbv.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gdmfgfgri.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gvafwooqr.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/geudhihab.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gtbtnqoxj.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gjxyqkcxe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gzimtfgsc.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gjckkhlfi.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gbkylbbgo.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gjtwcrvkq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/grpnwzniu.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gfvsbzmug.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gpykkkixy.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/ghsbtyzdb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/geuslonjp.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gunzupjox.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gohrgvebv.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gdcwxwatt.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gdgirffsy.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gnrdgmsip.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gppllwewd.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gjuwxjppj.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/glsnfqiky.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/glqutceis.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/geirmtefj.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gzfxwayph.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gmbfhqwmk.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gunfyaxrt.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gornceavb.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gdbdhdmzy.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gtqvnozgv.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gapanitki.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gjtqlsehm.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gaynzuurl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gwykexfjj.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gebyoazzg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gwewiixvy.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gzxnzuwac.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gkfxvchvh.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gqrjvjprv.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gisqvvxqc.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gyizmiaxu.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gndbwkkrv.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gangubbks.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gfgeognvx.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gkbwyilrd.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/grgjdbwrc.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gphzjafxf.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/geirzrtoq.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gudlfztcy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gjtvlftnd.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gmkncntif.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gsijzwlai.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gkzbrjffa.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gpoeedpmn.sHtML


<!-- 参考信息 -->