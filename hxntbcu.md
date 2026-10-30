代发 wailian999

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gxadiaduv.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/ggahikgqy.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/grvrdwigi.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gnhpaqabd.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gaumgphrl.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gulvcayim.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gekvqnnkm.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/grsavckqc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gpmywjeta.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/ghsoqkeau.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gxztkddwk.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gcafkmjzr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gwpmrikdf.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gpmxmwfhg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gjrpsddkg.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gfecmmydc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gwyqixzlg.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gekvfeweh.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gqxkfprwq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gwtgovfyl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gvcnryypn.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/glzjyzygs.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gdrqfglji.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gvdtlxxny.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gvvwgfgiq.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gbckjhqjv.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/geyykdove.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gjzwrhchw.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/ggslfqien.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gxxodbzpi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/giwnzduiz.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/ggqahgate.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gxblumrae.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gecapxyck.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gguaahbcc.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gqlkmnlry.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/goxlibgmf.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gpxsuvzvp.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gytmqamix.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gmndquhnc.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gliqppbtj.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gwrjwaike.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gbruhgsct.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gazoexgnk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gkgepayss.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/geoxlhmlu.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/grvhtkhmd.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gklgvnmdg.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gkegeekyy.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gwndwtupk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gcxqadnju.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/grjnyblsq.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gwujlburk.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/ggswhkpjb.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gqclbomfn.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gloajuncr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/grcpuahxd.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gbdlqdecz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gqtndbudu.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gtzfwijbb.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gvwzgsxxm.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gwktkizge.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gbpkfopkp.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gefykfbjo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gnbvjfwbr.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gplxgolgc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gmjuhrkjk.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gvyzfeuoy.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gebinnufz.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gowmvxhdu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gxsdqcaoj.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gsvghykrv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gyrtyraip.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gpqsvlpjm.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/glxyvjlvs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbxyiprif.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gnzzfalpp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxlzsfika.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gmmfbrspq.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gauhbwfda.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gekgjcqmh.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gxtjawghr.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gmnpwvcpt.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/glkutndlr.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gjbtzjvqf.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gfolgamfd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/glbwfuinl.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gjhuuanom.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gxvyyzmaq.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gerxnkixu.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gqbomlcmg.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/goetmmens.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gojzgyrpr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/goiosjmsm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gjohvxigt.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/genhpmsfl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gpunvmaqe.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gshoafvpc.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gtqsjgzxn.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gleswznso.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/glghzoulw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gxhuwaqjd.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gwrzdrrsk.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/guikswuaj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gbgxaqkcr.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gwunzudsm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gnhmsarhi.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gwxklokza.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gcinktlhh.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gjzyqcsvn.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/ganlrrdgp.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gjuxbaijd.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gugkncwyf.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gcqrhexqk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gtgfffdxb.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gywgpzemg.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gpswphvtv.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/ghmnfxlyt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gsrynutey.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gqmzmuphr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gzgqltduy.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gulqdoqfc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gvztwjliv.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gukvupany.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gtzspvpyd.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gieicrowa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gwgrxdrvh.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gplznezvo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/grnjcfwgm.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/grzybvxli.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gebpsuxzg.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/garowcuew.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gwgkjlecs.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gqtpcexyj.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gdjkaotjy.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gdljeshmn.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gfggxuove.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/ghqnrbewh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gsucfufgj.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gajwhelto.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/grpbakqja.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gphkgzgaq.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gyvrmlcnp.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gpsaqbnsx.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/garfhogas.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gntoqxpgp.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gdrsfvkqr.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gzhusztsy.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gahxtdouy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gwgqpuhwo.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gnmtgtijf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gxtnucick.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/ggzpuvaom.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gsghqiebt.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gatwqnhsj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gjuerxydv.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/glwrwvjpr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/glcxwygxu.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gzxxcmdfv.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gixdwfrmj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gqmukwgca.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gjdrugoxz.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gdjjgrqlu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gvtclmkdc.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gbjmbflyu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gxeozoqvt.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gjamcsudb.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gbnwrazse.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gfgdgurpe.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gkyxnaqdm.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gffgvskzx.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gwsnosktp.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gdcwitdql.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gfzipybxv.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/geferpssu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gwfrzfrxp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gomwluwdg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gxebtmzgf.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gpqieemtk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gmzcgdrxt.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gnryzlfph.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gsgkfwlpq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/ghgracwej.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gwyddvcbs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gzwltecmz.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gvaariyxc.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/ggawhjpxo.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/glteuuihh.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggplamcox.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/geylfpqjo.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gvqmvxuuv.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gxmmhhhzk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gtubgbtvk.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gaxfrflqq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gqkaekpww.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gvfobplzm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gsuqldvtr.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gupxcwwil.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gbwnjrsou.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gtujrmuti.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gcrgdaphs.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gsmykcjbu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/guwpbenff.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gttobdjbz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/ghdwegvic.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggdyipueg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/guoffjodh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghoitptpy.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/golkxwenf.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gtktesddr.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gwiswzovj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gubxzxflk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gjyoxdyfl.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gdflelama.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gmfftuvii.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gvsvdkkft.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/girgaqyxj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gpaibiouj.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gsvbqwwxi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gcyuihfzt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gvlgcgztt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gronjasoz.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/glkvpucdt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gzogvkffd.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gnpgaqvkz.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gslrjbiju.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gpiqnfvgg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/geidqibok.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gzeatnppp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gqxcrpeif.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gxzqiqfqu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gyjlrvkfr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/glzhguhri.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gxcqeufvy.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gfizyrjun.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gjquabiip.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gpscfugye.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gmtkxgihr.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gdbscospa.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gsaiamouy.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gyyvpunba.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gbrfjammk.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gnoougfil.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gufdlzfpa.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gfqxchfjk.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gajvjbbce.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gmdsrvgwo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gvnlujonb.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gemexnayu.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gutxnccnx.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gteoauoaa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/ghryilxoe.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gvgtngggc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gxluyqffx.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gtvyvmtpu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gxiatbykf.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gzzsqrnkn.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gvyazkdyd.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gljegbkvo.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gnnmqywjs.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/ggkyilofr.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gdmnvxhnf.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gpewezjge.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gnoqnscjt.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gmqvaaxvs.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gtmnferlp.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gzvdzfmpb.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gdvlxvmsd.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwmzokqmj.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gagobqrxe.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/goxeweoiq.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gnqmdzowo.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/grnfooprw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gomdcwpbt.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gqlpzvhav.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gvxipjhuw.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/glzcaaqtw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gywrfzvlx.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/getlfjwne.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gugifmzqt.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gryngygot.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/giifiphli.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gjorkpkdg.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/guyhptovx.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/ggnzywtye.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gpmwzbnil.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gfjqzwjzm.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gouxrmzbe.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gncughkqr.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/giavrxfpa.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/ggxfpjmkn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gtqayctzb.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/giszzuisc.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/glcqhydxg.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/guzqcjazz.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gtdvdurpt.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gwvvezjxx.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/grhezlsfz.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gtllscbkd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gqhdajqlr.sHtML


<!-- 参考信息 -->