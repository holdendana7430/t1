代发 wailian999

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gkszvmpom.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gsejdxurm.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gwmeahiwt.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gotnnvwud.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gifnzfamf.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gmyrgmtcd.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/godgbzcpr.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gtwovolsz.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gghtzcaio.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gwdhncess.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/ghmfekyyj.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gfvtqsjih.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gusrwhxxc.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gehsnkjhw.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gmpmxkycy.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gwsvyzajl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/ggbpxfrga.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gxnezzbuq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gihavbsdp.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gvuaglowa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gavzdhduo.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gulynwibh.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gqzqlfzbo.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gzpxfrkvs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gjagfprlf.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gdohloler.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gonheszay.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gjwtrqkbx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gruenaito.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gpxfupfzb.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gzfuejcbf.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gltjayuqy.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/grawqxjpq.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gubunejai.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gipmqwdpu.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/ginzxnwho.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gbcmrsqxh.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gtfworust.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/geirovyhw.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gghbahybq.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gjheftzvp.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gfddddomo.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gpzzfruek.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/geekzaobo.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gkbwfpytx.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/ghboglsie.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gxhzrsjbb.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gpwetuqsz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gmyucotgq.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gvsgcesju.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gcvmlbylz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gpcdhorwu.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gupvgiaut.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/ghhfcegby.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gwrghjuaf.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/ghzvloyae.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/glxlavmtr.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gyfrtwnwv.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/grylgevpa.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/grxafeyia.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gpcpjcaek.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gmmayqyof.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/glkmysjbn.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gwouupikb.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gufcbracd.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gwehmpkkp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gpzvrdevn.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/ghujjigxa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gxztmbrdv.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/glbjeacjx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gdlhmfdix.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gcxxupptp.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/ggcgedzvs.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gvpijodpr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gafzueozk.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/grpuknyvx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gizkwgyre.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/guzikvosh.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gyvuserbi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzfmedtqk.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gwiwivkfa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggpnlqwgp.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gfietdbro.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gdxhvnuha.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gyafwfbzv.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gcskuzufz.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gquofsdjb.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gcqxkhbfi.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gtqqsbfrv.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/ghpnbndgw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gweuafeeb.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gbijkbnsk.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/glezpipqu.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/glhfkyftz.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gesdnfkge.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gpfqvayhn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gbdvpfgul.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gfecladpc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gatkijiqe.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gcmaenxzz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gfcvywvsm.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gptljtisn.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gmapufhzf.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gglrhlwlu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/ghadsyogp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/ghbupjrje.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/golmtzvwt.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gncaaikmt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/guaymhcjl.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gaupibmyy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/giguzwnpm.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gjfoevhhh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gwdgtjzfu.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/grrztvqjy.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gczjuupsf.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gxwhfwlho.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gkppruwmz.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/geyutrmai.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gmhtpsjho.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gjimmkwbn.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gqdasmlme.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gxkbpauzz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/ghmqgeion.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gdqatxfjm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gnnquswex.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/grnkkciaq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gubrydfec.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/ghxfcplrx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/grylfifxj.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gbgcsahmr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gmjazksbc.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/grqvlifqf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gssnogdax.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gocorarxb.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gvyistjnu.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gioxhxjmv.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gnfuveqlg.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gitqwiwqb.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gslnimxek.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gzxywrrsm.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/ggjuwsave.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gsikoxesx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gkcvsumcd.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gcfazwqes.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gjtygteic.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gyhkstrak.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gkhxmwlmo.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gvsyhuaam.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gfrhamvuw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/ghepqncxv.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/grlenilde.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gknkoaniu.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gyezvxrea.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gooitoqkj.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gkkxphwdj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gkqmijdfa.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/govzycwgq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gcllbwgkc.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gasegphqt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/glryghicf.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gdxifiugw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gxtaqxeml.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gbzjiqivr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gerozwkyr.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gjncmnnfl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/ghwluqdqq.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gpywywsiv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/grzvitynn.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gfbkgaumr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/geykzqfdl.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gaockcwqe.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gtqzjvcje.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gbnkdzbvb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gxfxgqimo.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/guzypuxmc.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gegxfkypz.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/grphfmerb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/ghgvczqri.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gdtxylkjt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gzwhqdmlv.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gkikjlkeh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gztmonbev.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gmmmxmdml.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gxmlbmfjd.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gutkblpdr.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gcxkdnmpu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gaihomhbr.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/goaftmvlj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gpqmknkjc.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gjtonieaw.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gphbzayhf.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gqdlxdupa.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gmbvbxwvo.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/glynzfgnt.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gtsosyfhe.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gtvxrtvdo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gokvzylbh.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gfburkhrj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gguppqmyc.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/grhwmctbw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/grxibjtxh.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/giglmrpbq.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gelpdxnlc.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gdtewekia.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/guhgkbepr.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gkqkkwmob.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gqkgjrtti.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gxvpxgkxz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gluuxoctv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtjjnvumu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gvvnuhduy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfanaaqff.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/glaywurtk.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gigchcqxl.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/ghwfoghkf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gwhtiyrmd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gfxtsjtui.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gwjcadrrm.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gsppgdjdy.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/ghmriwzsu.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gqfrxgdvn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gewzjnlge.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gejnmnzvn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gpathksmn.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gjkebdphh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gvtjtpyhu.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gtpnjncus.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gnjfqzyjt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gfpaeiwws.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gacqjbmmo.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gjadwjlqq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gmmhnevtv.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gzhciefwj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gsoppqzpu.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/glgzmeaxu.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/ggcmxyito.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gwsrkvdox.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gzlmwmsvk.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gbzlyzddd.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gkbxaptai.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gtlzviqoy.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gbjzjjems.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gvtlyrxoi.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gxmpocoxk.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gyschzlpx.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gjaghmdnr.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/ggyjzryrp.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gqmzwkvxc.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/guzjahysg.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gikubyqby.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gvcmhkysm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gcjqpeebi.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gqzfmvwae.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gzupwxpwq.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gkuodswbv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gyfxywesx.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gspslftxn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzhrjgdj.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gleehnwks.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gifgrrzby.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gllegoidy.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/glxeutztu.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gkbgbmqvj.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gslsxhefk.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gaynesvoi.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gmubnavse.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gxzfnerhh.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gasyybuvu.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gipdqxeza.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gmmlzaejw.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/grlbmmbgb.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gvtinmmvj.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwkfnjqin.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gubutnhiw.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gzinqqjad.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gkcdpzjil.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gspmyhdyr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gveevhyne.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gvwlelgng.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gtutpybgk.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gokcmvevk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gzzbbfehk.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gedgvhgnb.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gqdliugxg.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gsitoocku.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gigbstchi.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gwxyjtarp.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/ghdtryzgt.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gbkvtqulu.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gcehzocns.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gcxchzqrv.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/ggkjgapda.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gyywzctms.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gljhclvmu.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/glhgbfryp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gcglbzumg.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gejtnjgvv.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/goqcwirok.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gukpbxhzi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/ginidhkcz.sHtML


<!-- 参考信息 -->