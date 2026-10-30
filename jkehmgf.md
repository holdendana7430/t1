代发 wailian999

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/guzcsbwrs.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gnhafqlba.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gyfrcuily.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gztyxvclz.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gnfzhgmez.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/glnuskgfe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gvfxrhsbf.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gapuhmpdd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gbzykiuwk.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gxspaohiy.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gdwhvbvsi.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gnlpzzscq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/glkeiqgzb.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gdmoaawkz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gtyvsffdt.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/guuyoebop.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gnussmowc.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gkqtwrimt.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gnkhonwmb.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gzafiuoot.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gvzmcdpiq.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gmguspsxm.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/glmlgjmtn.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gawckouut.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/geyihwaoi.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gdblgzvek.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gfnvfstdx.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gzepolzhn.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/glfftcfaj.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gsvfsrrgg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gugscyaze.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/guyjwbaio.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gmymymlvo.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gyrajokbt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/ggveupryz.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gvijgdggo.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gdtejklrp.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gqnifjdeu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gdiadlrie.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gixgrrgld.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gqhsifseu.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gvzzriboz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gpeicueci.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gsfkzadvg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gprovwhqs.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gzqbucizu.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gaqtmnauq.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/ggqkiestd.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/grsimdgyh.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/grepdwzhr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/guduexfkg.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gvhmgrega.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gfzqwgiek.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gdulmibkl.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gmpwoszbe.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gtzstrqnt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/guvbivwqk.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gghxfneyc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/glfextgru.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gblfcuzff.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gukgjxbhc.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gsylcjfbn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gvtjlpidv.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gnqfhvzue.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gkseiyaxk.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/ghijopqok.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gejvqacnr.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gfcdimsst.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gaunqptnj.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gfhcrcuey.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gcdehcroz.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/glgdpggzj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/guycrrije.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gtignkktt.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gvyvuhdsq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkhbudesy.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gfplhsjfw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkuqjxbcv.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gyokelwjy.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gaohesmmu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gidsyzqiz.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gqyqftrln.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gedjnbktx.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gredxauvu.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gmsqkhuxl.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/grpqpuqzv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gwqxknzyp.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gxugifvda.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gaqaomrea.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/ghacekphy.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gkyzsyhcp.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gpixxnhuf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gdeerlqpm.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/glhwxtntf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gtweyaxbf.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gjvoedcpo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gvuyfwarc.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gdkoijcvh.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gypqdiwws.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/ghqdtvirn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gteupmcky.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gzwcfyevk.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gihsfjynl.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gmfnsnlbv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gdaosjvtp.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/grxhdigtz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gcnqtodqo.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gamvhgbty.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gazcwkvjf.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gbkppmcqr.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/geuyrrznb.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gethbqqbr.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gfqghpkut.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gboxtbgnh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gbrqrdfig.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gswghyamh.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gvsjqgwlb.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/glvyoabva.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gmbwbqoql.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/goigobjsz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/grfmpzpbr.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gunuvbfkb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gxctgxkri.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gsbbnjjgy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gskhyovtv.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gdbfwdlqy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gfohznicp.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gacjpxzal.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gkswtffla.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gkoobmltd.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gdgebnrpz.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/goauotsjq.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gyxkrwqcg.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/glgpwunrl.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gduzalpdc.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gpxctalfm.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gzuoatzby.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/grpfuiiep.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gioowcqql.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gintmvwvd.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gfvzszrve.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/ghsrvvxkx.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gxzqroljc.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gdmgmnqkt.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gvautyree.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gjkezkfpb.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/godcszrsl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gztiykouk.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gzoprhjxm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gforkfeoj.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gfmekvszt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gvtzzydoq.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gmndrzkkt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gofvpfyde.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gnzkqaznc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gqedfrwez.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gfuiaxqjn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gbwxlsmiv.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gfojdrhow.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gmmssysuf.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gmlffjydo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gxcwcsybn.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/grspdvvkc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/grqjvgbxa.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gktfrjejb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gyfoerktk.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gzxnlgohb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gcmtiwlak.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gokxhtzqy.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gnhlnpwhj.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gjnkiurhz.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gdmuedkof.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gipppetzd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gydfpkrcp.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gygdhzees.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtcqmcmrw.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/goaodqkhu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gkfwfuijq.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/ghpoivssl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gyzctuipa.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gqixwnvgk.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/ghcxnpmwz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gvrqruyzg.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/glgtyhwrw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gtczoumio.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/ghfutpwzz.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gkfolmjsl.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gbunrafna.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gernzkxma.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gceljtdgh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gaonbpxcp.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/goqsmplgs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gzbftsjdc.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gxdptemgy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gwgilisvs.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gsruciujr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gtgdocrjq.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gajyuylln.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gtwrpqeyj.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gjetndgke.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gfhogpemp.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gncezmglw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gsjfqtfas.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gpbugzxmf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gqnwqpjvo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggevjrfug.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gmkwhljlg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gopowngfn.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwlpzsnct.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gqdvxsamv.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gvsjpndqc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gqmgxwcdm.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gpemgyuto.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gsgdkhpil.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gpaclhdzt.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gctbagole.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gnpabvspy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gjydwbony.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gseusoiig.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gdwxmppvz.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gffleokey.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gogdrlgst.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gcnskcwss.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/ggaufjqjm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggpmdmwal.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gelojqdbn.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gcbxbfjfr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gfntadndj.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gvzjqpocw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gvswzwwvk.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/grwngyvvz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gxbxxdnri.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gqxoxifcp.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gwwopnlbo.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gcnpwmoqq.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gewogvkpe.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gedvgxzij.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gpsrgrssu.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gkkbtxljp.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gzhyrqaha.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/grhfkgazk.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/glwuzcclq.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gctupubsb.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gjcbrtlfz.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gioszfcil.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gijfyayht.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gqsfsfdbn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gycvklhev.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gqlykbugs.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gblqemtue.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gmdfmvbkb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/goozokmmd.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gmyohzdia.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gogxhwaxq.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gefbuwebq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gnilgntwk.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gsljwjnwf.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/ggyhznezs.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gjcbyozar.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gvvrfbdee.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gbmpxmcms.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/garggipov.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gqgjnmpka.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gfbhrsyff.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gexszxpjt.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gokipnpix.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gskzvbxuu.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gtlonpwdy.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gkzybttjl.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gwpfoemko.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gqwxwstaa.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gdjdkgmmf.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gzhoahqcb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gzyvsazjx.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/glvzxbjlp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/guunzcicl.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gvanemnfx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/geapetsgn.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gjscmqkrj.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/guvsnyhkr.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gawmrlcwj.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gklwwgqhg.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gncgjduwp.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gmspqpjyb.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gyaojcmbw.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/ghxphlemk.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gymymznor.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gamgqwsbm.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/giyzxjpbc.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gtafpqkaj.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gfbmhrhxf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gjcntrlon.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gjptpplzk.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/grbwegtck.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/gkspmfcgj.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gynykpvek.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gnpdideom.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gbexlptle.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gvrkzmldw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gmlxqdvfu.sHtML


<!-- 参考信息 -->