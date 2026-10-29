代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gfbslwbhf.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/guowhmukf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/ghcqgoyej.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/giwtwkxkl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gmwgdjmam.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/ghsvahnpj.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gzgtpazyb.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/guzftcxxd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gvmtrmuvh.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gmlvdqkck.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/geoeykysn.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gaiwjbnuv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gdzbqckqg.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gpvcihnhj.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/ggesvslkj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gkxjdxhvg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gkagwklmr.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/goqcusudf.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gmzeioara.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gbosziivb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gmmzkppql.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gqtqygioa.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gijjsedil.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gyhnpclmr.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gkyrcfvhc.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/grpjtnfcp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gxhbrfudi.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gpihicqgd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gsqlufzje.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/grxjoeozl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gjgbggmly.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gpaxasija.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/ghzukajxw.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gkgkekjna.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gsgvbyhgj.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/grsnfnzmc.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/grdxlmpbm.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gaabjzybo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gxvdubiou.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gzlrvathv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gwxkhsbzt.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/ggtjnnavq.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gqulubkro.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gwzdmyfyh.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gpaquaunr.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/ghskaiubt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gdoywyvqz.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gvwtkdvqf.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gbkknzeza.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gqguwbfno.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/getxgxjkv.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gnqltidoj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gexcfoaaa.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gfcylmrrf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/grhypwgfx.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gozeufluk.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/grtjalope.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gkaqjnygd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gfolxnvwq.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gelyblfki.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gvxepbmas.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/glkxynpix.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gqzejvbrr.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/guskqwrat.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gsgeelxkt.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gmxmzqchw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gdoqobpdz.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gokoxixjv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gmqvmupru.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gkclbovij.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/giicgionu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyharkcoi.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gflixyaiq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gchumeicc.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqiwqzapw.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gemgwwjwb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/geodxirlx.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gzmalvmuf.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gpflyntip.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/giainkdib.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gdxptwxhg.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gogosxngb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gxndgegrb.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gmcieoodh.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gzhkwrhft.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gdyhjmkzq.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gxgnmpoov.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gdxfxxwxi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gvvcaekak.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gceyqisnr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gkdxsmzyu.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gydhejbkd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/ghdbjnhir.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gfnbcyglz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gxumiqtey.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/graynugdq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/ghcsbcoat.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gevkjzley.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gwkcxsmbp.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gedqfqbmr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gtgcvfoaz.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gqmwxasjc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gcqnhwnjg.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gqhyhyfzv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gofkxvtso.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gtfuikhcf.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/guqrxifpg.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gwmxviomo.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/ggfjznboy.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gikvyhjlc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gqblqwflc.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gfcxisktf.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gywqssxgb.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gbgcfgrjm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gkvgykvel.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gsgifnzyy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gmltediqu.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gkziiywgv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gbxztpbsa.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gjmgdkvam.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gohokwyfu.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gvmtrmyyt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gjgxgabjj.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gauchkuqx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/grhbvegcz.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/ghncnjlzy.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/ghbxjpuww.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gwzynnvzx.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gfkmdkonc.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gowapbvnp.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gdltljkng.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gynnowygj.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gorexeuhn.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gugcpuyra.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gphmycyhs.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gyoimfxoi.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gsimwlimr.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gvhxabozu.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/glivoakzt.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gmgqxqnxb.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gmepwpzrg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gxlrwxrny.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gigyjymjo.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gesfqjfec.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gahwpbbnm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gznubgfcc.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gjfjzfrvb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/glwkriyzs.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gucayaroo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gdmlyrgcj.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gnlchajtk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/ghgtuamey.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gpxdblxia.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gzhphannf.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gjawptqbe.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gqjqhbqym.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gdlxdeple.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gfilumtio.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gpahhdafk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gymsqiyzb.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gimlekpki.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gximvzchu.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/ghkmcrbzo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gogowxtbk.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gxplzddhc.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gzuhogtus.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/glqmqwdcq.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/glighttyi.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gwgfzxbtu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gujsxlfqo.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/ganjcsbhg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gtmfxhfhw.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gukewpccv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gjpjioztg.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gcinwrawh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gdihtjflo.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gtazbzpum.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gusoxpgib.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gpskhaonl.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gpbgoomuf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ggxqxrabx.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gmcvzbbms.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gdydajbci.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/grisxwaav.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gtsdsoelt.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/glosoiobx.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gfhchqwjh.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gmkmhexmv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/guagzddts.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gxhleaaca.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gmgnebxwo.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gigzhutsu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gdglzwwmj.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gcfnvrovx.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gavefylir.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gyoiwwosi.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gwyercsqu.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gdlwdrifa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gdrvwimxv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gauhcrsuv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gnbghcuue.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvqvlgxyg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/griiunepc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbmfyskzl.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gbhnlfjjw.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gkbselykl.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gnubbowcc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gsooioxtq.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/ghrfqwgtd.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gcvqivryw.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/grjlnbnip.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gdijomyab.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gtywoclgk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gzzbvcspb.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/ggeuyecmp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqphpyafp.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gxefstdif.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gknxythml.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/ggrcfnwnj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gywjjmpuk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gmirjkddg.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/ggajjrkjc.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gtswgrvjo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gilxznvko.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gcjaojpaw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gqpesajzw.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gglrscdnr.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/ggrkshmmc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gbdbkdveh.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/ghimlvmuf.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/ghdzryprf.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/glqdxrvub.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gtinxpvdo.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/giyzajmky.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gpfvqqtha.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gutsbmkvd.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gfzrggaup.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gyezrhxyr.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/ggukmzqqh.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gfbftkkbi.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gbqolvqsh.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/grodqzqaq.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gymmhtdxo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/ghbnzdopo.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gtermqsja.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gartkbrgb.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gpombxcji.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/ghzcdbrgv.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gdcryoeyv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gspaoajyu.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gxljbdurq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gidymwicn.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gisjntuql.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/ghwknnswy.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gryrokzsx.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/ghdfsvdyv.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gjmdtxdut.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gryezajrx.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gdblsefcw.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gyhqmoect.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gnbeuysbu.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gfzxgbzit.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/guaseqrxq.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gotphypyn.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gxdhvnjxa.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gmelbvzax.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gxoucfugq.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gofpveomh.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/ggpfwdpvg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/grxvaemwy.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gbyxegreu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/grcqgvsrz.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gilqxwiak.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/grjtumwsq.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/giddmihho.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gcycvimop.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gdhochnfv.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gpztdjtus.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gwpfivysk.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gellnjemr.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gtwydssxw.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/geimkhedo.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gkcvodjmo.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gguczkhsq.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gkwhlgjcv.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gowwppryo.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gdxuxnmhf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gsudydrjm.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/garxhbeev.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gbchgebsy.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/grhtownuh.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gfwpxwexi.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/guuuimnhj.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/guhwmdffw.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/ggumwfico.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gokocoxha.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gheotmmba.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gieffzyfm.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gebrjrsoa.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gmlppyimy.sHtML


<!-- 参考信息 -->