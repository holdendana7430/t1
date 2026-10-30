代发 wailian999

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/geklbxaor.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpoyggqc.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gwkhiaoem.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzhilkqb.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gastnfxqd.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdurpijj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gezgfeqta.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gvjxxxppw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuekruzw.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gbkwjerql.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmpcjyjk.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gjbfwmyoy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssxptpbx.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnrkiqjv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxkcnlfc.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghminvvzw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxlundan.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyimfynq.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggibggwmn.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/grdsodmeb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/goehkarfv.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnnmbxqk.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gaausurkb.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gfvdzupaj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvsewpwg.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gutewbogq.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkesfxiyh.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfqtvzig.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gpqebflwc.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gllqsugai.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gewwetftp.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gvvimirhf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gwuwxwqqz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyzabctu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gclpnlodp.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrgjnqbe.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/giptntywf.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxqhmzkmt.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gwbhgbakn.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gzmhqtuyv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gksnormrr.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyremuvs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/guzsjzmdp.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gztkwbdgn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmhdvilx.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gvhoyickk.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimclomrg.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfamqmac.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gsggdjruf.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gnzouakph.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmrosieke.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gypuwmzbh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgblflfg.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gvyfhvwzi.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwexbidri.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhsrtygp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwscuqua.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/guxuwdwpc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaemssjzi.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gnmgqzttn.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/guqhcegyn.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/guakdnezy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtknlmjmv.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpirhlfjz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/glzdlgjal.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqwskrlyo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gysffzzqj.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqlcpupk.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqbtnogz.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/grazqkltt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/grmyguqta.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxynyxbt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyqvuliiv.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gqfdktafs.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpbunizc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeijyxeq.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/goffmaskp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoyzihkw.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxqjldlwn.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/ggffcbnsc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzgvycsnz.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzhfqpxz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobthiiig.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzufwknp.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewfkebsw.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gszfsdqcy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gmwvdacjn.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmkijgaj.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsjelfsp.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggowuzsxn.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqffsfgw.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgfwuqip.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gjswlivuo.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/glhoffvip.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/glmycpbzv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmfogtby.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpzvukah.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnihixei.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gdemqxfjy.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guliaosxy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgtgjtjr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvxaeqrd.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gumxlpxei.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpozkwjdy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrbkpmtw.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvpxypkr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghysxxgcp.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhsaaykx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/grfcoenjk.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gamdazmef.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/geezkgtep.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/getknetzy.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gidkrjzde.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/ggmmrsffw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvhrzewn.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgcdyroy.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqbejxbi.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gqaodlohf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvxtxiow.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/guwkujbal.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzbjhqzw.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gfumfnnuq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gihejtgyt.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/grgtkqkud.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gtwfugvwm.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfiocdnv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gdqhheirl.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/geygcrkgd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyqezxre.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gaopghpzq.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gpkddwjxn.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gnzuhogdi.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhrsuypr.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofwrsbmo.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/geprytypu.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusuuxymf.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gqkflobed.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpmjjiavo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/ghajzpele.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gyqqqaabm.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzjluxtn.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhtztmij.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gtftxppgu.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndtcaegm.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleugrfkl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpnxmnzi.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gjqdeosgt.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxtvlfvv.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfbckwpm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gpcvgzotu.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbosbamej.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyrafkkmt.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlkdmxtk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuvwxjzu.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/goybhmnhw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdauicpuj.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsxusetw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gckhebpen.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gtpszkbfu.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvlpfupa.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gremfgpkj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gplhcemyq.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfwypyhs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gsnvaddbp.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyspokbmk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gdlwseedl.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvfbajbmo.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gbqapuipw.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/giusgqhxc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoafwbew.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/ghrzukygn.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gryrwomle.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/glnmoiwvb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gsngqlcpw.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gsosygqll.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gynbiovzt.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gzoddrpae.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gakqckahn.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gekyvrobn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdihmdlqh.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbvpeodb.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjjevhxnh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gcpufbdpf.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gagatsnqx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhwtqkub.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gcidwlchu.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtufpcox.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gcbddeabg.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjgvufatm.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdtfagcp.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbchlhbez.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gcquuxfoi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghudrbzrc.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxqxrssn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gugwnfajp.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszvjdosh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmseidfa.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmofgate.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gubnrajjx.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gwpytedup.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrijscsx.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqyjhlsv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqbiepun.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpfhdvhi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/grwhuodbh.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqefktgr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhofsnro.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/guilmhqxg.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gzpuzkvgb.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gobtynzix.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/guukxjpld.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisikodqs.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gdccovips.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gwfvclzfs.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnnwmxqt.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/govnwvhwt.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gixovnvxw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxbxcbcy.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/giwwgnqlp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gbbjprpoi.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqooxmwk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjptdugz.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlfwarqk.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gekeyqiuu.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkqbehtyu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmyrhcwq.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawllwxcn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/ggpeiovau.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gzljxttgb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuhmygjz.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gqlbuvjdo.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaetsbzm.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gmwpfiqnu.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswsuzeyy.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjdodnqu.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpdzlaol.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gfoolkbma.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrqsxmvh.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gkkpiqdjm.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjeyqcfk.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrmucfgb.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gdejlrfoi.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/goxtcofbm.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxcwuzfa.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/glhlfsant.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gqeeoqzsw.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyqmchjg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gslzihjef.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gaatxytma.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunqvyjhs.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/grbgmzjgs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gcxydtuww.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkejgktq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggatmwjfi.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gkikxrani.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gswhvgfot.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gvsgkoiee.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gucytcoys.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gtakhidrd.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gvziikotd.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvtkgpis.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gqlmwbxep.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfswbgekb.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gvrasdsgp.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gmwmwmbad.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggncviepn.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gwhulfxat.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gacaripei.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfzshelo.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gwhcrhwkn.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/genuhvowz.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/grjhwnrjj.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbncohnpj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gsemadogz.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gvxxuvyhd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gwldstloq.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gftgcfnjd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goztgvvzs.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gozxmjwvg.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gtudbyuzj.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpatfnqf.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gotmffyyv.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxxxsfme.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyzfddth.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwelqzpx.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyodfimna.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsrfwaof.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gsniacifg.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gkonovpfd.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gezimzjia.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapjdavpc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/grxnjobxn.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/guvzflpip.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gkyrfqyiy.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhuljkrd.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdowjqszp.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gsaqdxeod.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gymspbijd.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gsydrolje.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbiqiqtx.sHtML


<!-- 参考信息 -->