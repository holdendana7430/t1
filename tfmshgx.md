代发 wailian999

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gjdvybwah.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtuyyfdx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gsksjeyin.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbalypnej.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmolerebj.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/goszhugmy.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsrvmfii.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gboxwuqyb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/glzmarchx.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gelqdnwqu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxndhwkxr.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gdakimvuk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gfazmubhe.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjgwymjb.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjybvdudo.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbwsgryc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gmphyxqij.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoqxgypn.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqkqqbce.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gafmurlsy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gstwfxfec.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gkynzwdqo.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gffzzbjbo.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gezqeiztk.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/guqvvijmc.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gesxajqco.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gungeoijg.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjrpyxbj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/grssmipdo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/grotcggfu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gwidcqoga.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/goeikezxh.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/ggchlcrtm.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwgjhsnjt.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcxbazks.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnitrdirg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpihyjyta.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gsfmuwwae.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gocpmprrl.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmltowfzd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gimleyvzg.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkslgttja.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gelpxannu.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/ggklkcmya.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gsrnjiafg.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihdryenf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gupysguvw.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/goasxqren.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjequilj.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeilbpfy.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrpxubxz.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gigjoqqzq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gnwnuljta.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgruppkn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gawsrwnnv.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gweslzoyi.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gpqiubgsq.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/ggjqmdola.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/geqhirokh.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gzmtbivzz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gekoamonn.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gokxffdjx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzucgfjtj.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/giojdrssm.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gzqhonrxf.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gjswvgasa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbpjtfff.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gxigdpphk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzufxyxqe.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/ginhjmnhq.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gfepohpbs.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gsbqvfhjr.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxuqaxeh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpwmphmg.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzazgekep.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/ghgfhdchg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiupyyby.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvvmqupr.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gnacbjllq.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggixngzxs.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gsossogsk.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrofbbjp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszrcldxs.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/glndpmrcf.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpncwlby.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gholzzwdd.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqbnozha.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbvbrzpk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpxzrtqa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuxzvxos.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiagogwd.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqmbsqac.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyculmwg.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfnlxqfu.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gxjxledfw.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbbguxwbf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gywnrrsjo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gmzmwuszr.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gcxhhliuz.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaywyrpvq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvaygnsg.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbnitbio.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxadvhkuo.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkfyohrq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsmjydqg.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gengojkql.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/glqiqgltt.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdgpkwvp.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvqvdsyc.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaxocqgd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gezxbbjkd.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuxncgfn.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gzmaiibqn.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/getfugjil.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glemuppkd.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhwqinqc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyjmfolr.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnkprdva.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqovghlld.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gmylcoaar.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzikmwidb.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gzprdewby.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigmdjxod.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gmavplame.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gnwetmqso.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmddojky.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeswpinj.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gzcfligyk.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gaybfdbyh.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlysgmli.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpubeicbp.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbrlrnnj.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyvfdhph.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhxdqsbz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gfpjjlrgv.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gajxputey.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/ggpcvista.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvnmnksu.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gqeovnioq.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzimfkwn.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/grjceohwx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiezgnla.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrtrfxwh.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gmegwfqlq.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gasjmmait.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gqtccaxok.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjymavna.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxtqyjjm.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gksdhpkni.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddsvuelw.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gslszozqj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gcnijtpuu.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/ggsfzjyth.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gzhnbbccw.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gaiofhipf.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gtnsusdsx.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjeabodi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gregkwqdm.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggchjgnid.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwqnuoni.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxycxjecu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gauftvbwk.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvjgkimox.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gvrzwhoxl.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gceniyzet.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gmyhgjqsy.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxvewexd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvdtewxx.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gaukysynv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqqtqrnt.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamqufnzu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfgponxsd.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gfnpxkndl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvkiwgmz.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnbecoqbb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/grrfaooai.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzfavkmf.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfazoyvs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwmwtwrj.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/ghceyiwku.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkyvyvsp.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvizfydg.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gbdakdxfc.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gdallenps.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwywsewf.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gpwzqtfko.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcxqmwto.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/glairgxxg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilvbcksx.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwrnswuu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlsfaxpt.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/goayyqxcg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfehatdej.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagvecreo.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gyyjrfgzu.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtmqoenn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgkvanyv.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gbimnhjut.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gefkjynii.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gygldzgln.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gqownxmhn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/garerkonl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gakhrprum.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxthutbd.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gtncuhmfi.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gjqvwfspt.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gougpntvo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/geyzevlmh.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gahvzynhh.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gnievwzxa.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gonkelmci.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqqtakdy.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gqjikxwdj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvhpibbi.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjdjgysp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyzhxjxl.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gjxzfpfxz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gijtlbjco.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gncmojjxt.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/grxfagyxg.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhnlavee.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/golkgkupk.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgyddwjw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpfanwpi.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/grapbpinh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqefhggl.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gumzbsrsx.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gybevcghp.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtvzjlnh.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gdwtcvbhj.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gewarvhgg.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/ghbzwaava.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gluruwlkx.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gajwqdmcf.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghygfjnys.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/greskvqbm.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeylvfem.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/ghlliidzg.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gvkmuavog.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjbavnog.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gndxjoucl.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqabdgxu.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoyimsjr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/glnanqdss.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gmhoozyjv.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmpoafyb.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikiptqcb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmwcdcqw.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/glojhvrat.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuvvftzv.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmpauhxh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gddxrkwpt.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/genumqbnr.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gveselnkr.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/galfgkwgg.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gudztzatq.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gesvznnxb.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gsnshvovf.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthfynzfz.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gihdxftsm.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gnvbhjguy.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gffowlcxr.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gircfibng.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gffasduau.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahanvnom.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gdovbjizw.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfgampeg.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/galddwlav.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gifwuegjb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggikvghkr.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgzpbydb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnmtxbbs.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbpelkmn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmsrprxz.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gthnfdwkp.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gkvbglwsk.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gegcnjzra.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtcagitj.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gpesyeubu.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gefnmwbez.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gleyhnfqf.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzujfgqtx.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghecwoihj.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/ghliucjol.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gujusollt.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gkpuaaqnk.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmbuucne.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gmazvnzmt.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/ghkyxscxw.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gezwqbucc.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbblbwvja.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gglqdyclo.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhxjqnkd.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gecguvmjh.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gaypfuorl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwovtiaf.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoqfklbb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiabclbc.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiouqeiz.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gfaeururv.sHtML


<!-- 参考信息 -->