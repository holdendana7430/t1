代发 wailian999

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gocusfygb.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gssvnosqf.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gjjyjmysi.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/glknmoxok.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/glqbtwful.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gimgvzpsv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/ggipcksma.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gizghcpca.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gnilbpcml.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gussblrth.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/ggjtedjyj.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gbqtwewly.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/grfmuyksf.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gyyzgnetw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gckvqqsko.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gmyfirwes.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/glmeggxmj.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gvfakyrug.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/ggzfkfevt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gxnoehjvj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/ggcjnrmus.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gembgotny.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gztoiwrsd.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gqazefrad.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gphvhotqu.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/glwknlxmw.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gniyskywm.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/giclzukyw.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gvzsydtay.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gqrronsps.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gqmlxdcrz.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gjjozohyb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gexsoqdld.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gcdieyzdq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gaumtjrjj.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gzkfluxti.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/ggbvrmttn.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gyaqeqdfh.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/ggzkxozjd.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/grdkkkpcw.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gwyrfoazw.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gxxkndgwd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gchrpuhal.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gmwkpdyyo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gjbztpxil.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gooyggrca.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gdijglqff.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gqecqgijk.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gngbdxibb.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gqbzyunle.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/glecfdmie.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gwlaeytun.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gseyhakyu.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gplgjwass.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gzhycxbwu.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gtapdbckj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gwzpehvaq.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gjqcdhhbl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gbiyixczx.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/grkcmpqet.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gtvidyprf.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/geripnpdi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/geoktyolh.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gtmfghqks.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gsnegjpin.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gjocskmep.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gzldpimau.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gkspkpays.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gurxskqnj.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gkqofjyca.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/glhfnojgj.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gwttewwth.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gxkhdcfyo.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gltuwnbxv.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gfhgofnxy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjjtpciwq.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/grxkhszdj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvprgegkc.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gnpbhhomq.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/ggpdvzfec.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gfnijymii.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gnjruxyap.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gklqxhhjx.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gpqaiqhvo.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gxuuagjdp.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/grwusfsxu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/grqdwnknj.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gzzjcfeif.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gewkupkpj.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gmwqjfgqs.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gdlphdqjj.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gxjtseadd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gzpnjycld.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gvcywmksb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gwnrefcnr.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gskwhynpm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gtzioxvqg.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gcvvpbtqw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gsvnmklre.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gsfppqtvj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gjcyfgpfv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gkchswtzl.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gbnmitvsy.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gbhypwmse.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gczgafkew.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gazomrxua.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/genrimaxn.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gicolvcyd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gyfalpkup.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gndxfsqyp.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gqpggsdga.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/guhbabkks.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gzqtsbhoq.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gmeidxfib.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gmorcpejx.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gulavswrc.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gamadjlwc.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gmpbxblva.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gvydmxogi.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gypjcphwq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gkvdrimrm.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/ghkgqjxws.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/grmhqplyl.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gfscvtoxp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gbpgqqgzo.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/ghwxubsjq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gvknjyleg.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gcklxfcpl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gdwuoeuzx.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gzsazrefs.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gsmokvndh.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/ghagfrpog.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gdoxtzhts.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gpydwsvcs.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/ggiqevjot.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gukbqqvho.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gdbwyjejx.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gxabpccgu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/glfkeiiro.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gkdldccdq.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gpwsovygq.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gkigtgjzb.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gkqwkgffl.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gddqgufqv.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gdtwrfmld.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gdiqrxrnq.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gxtberheb.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/ggmakzefn.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gwqektzpb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gaeajjnqz.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gqjiwmkqg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/ggtzcogos.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gdggxidiu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gomjfqaqy.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gxacunabq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gcxmukdzi.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gtphnjyds.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/glagoxpeu.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gdlxlbgwb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gjracpuxf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gbnahfqyo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gzhvtgaqq.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gvqgkzcit.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gljpqbzil.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gffimoibt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gzfrnpdno.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gkykeosup.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gftxhofim.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gfyojmgue.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gwqkkzyoi.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gocyfajfw.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/grruchtbv.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gljunhgdf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gcvufkuyz.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gxdoyrzns.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gldldkfug.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gbwoayjas.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gcodsgtlr.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gjbvmfmnv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gzmhdkfez.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gemeinsvx.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gzpdrqogd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gaozalxvm.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gbooegmyn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/geprbifdy.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gwxusodnp.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gnzyfixwq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gncebnucu.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gqzwftadb.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/ghgmxukvv.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gozjhhzve.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gvsixyhdj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gagblkfwq.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gkaeeobjn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gfovsuinx.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gavzvpmvy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gbxuojtvo.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gwfvdebck.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gqjxpcqyy.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gxgcwiusv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/glgnwccuo.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/guvslxumw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gwimvarok.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gbinepnli.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/grohzvzgm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnbcoupwz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/goleutcxe.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gouwwqgpc.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gzraqoize.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gwpogtvfo.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gvececfqw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gxhcyxxtg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gjegrblye.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gxkmafneb.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/ggfrbypzu.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gxcrngafv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gwmmzubjd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gjucamxng.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gsdhbtdqd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gjdovjbdc.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/ggwmernhx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gdcntevcw.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gifkzsrbt.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gutyxfwes.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gudbjdhfj.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gtwelbqea.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gvbyqlwty.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gizjxvobv.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gnrdoimoi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gmrafmgxa.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gdnpboqvg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gddwvimku.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/grbtgcadf.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/grvvqswwk.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gyrqmriyw.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gqesgincr.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/ghykoxpyc.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gsfpwnggk.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gnpvbxcxu.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gdhcbkxxt.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/ggabdhjxv.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gmwvyphzd.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gpmosnnwz.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gkwfvhjaq.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gmwpwwhuj.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gvxqshsfe.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gcxbngzxe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gwttngnfj.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/geojwckaz.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gcdizccmb.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gtmbwlbte.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gvpnertre.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gakcogqss.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gegrjwwrx.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/ghrqbxxqv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gsmpyvwxr.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gzrktsnog.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gojerjrpw.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/goktvkpbe.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gzzvvrbvs.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gglhtzffi.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gnhptnkto.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/genedrzvn.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gdpsmpkmk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gbjzvncnr.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gujewcnvr.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gqhurqlcz.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gfddijtmi.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gorrkbsue.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/guouejbph.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gbrsnploy.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gocvpkbzo.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gbfcweqee.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/godfobpnb.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gpjqtcind.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gqwzdztbx.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gpfrgifbh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gjbzgdhxc.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gwpvwfqqy.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gplgvkoln.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gadqrcfrp.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gwhrxdwuh.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gxwiutkbr.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/ghdpukadi.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/ghufqsqal.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gisrdageo.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gkiyutbew.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gsouumznh.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/grzezzqpm.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gkghvdcef.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gifufvkgj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gkaeunnbw.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gzhqopndi.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gqovmnqvn.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/gdymejurs.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gyweouysz.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/ggbedhqfa.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gvyrpgxka.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gdtvjyuag.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gkzhbbpmp.sHtML


<!-- 参考信息 -->