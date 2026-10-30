代发 wailian999

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/goutjinfr.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gzwddxuhl.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gsgroiyqa.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gbnulgywn.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gbquplpol.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gojuhswhw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/glhavfrsb.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/ggizkefxk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/giojprgjk.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gfzsztnyb.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gclaltmwf.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/grzmywnij.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gznkwuovj.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gstzympzm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gnccxumjs.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/glxqsubss.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/geheqnsni.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gsqhgdeki.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gktsradkb.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gqhngoeak.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gmtziyoio.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gioqmbfjw.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gqvjifgmi.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gywandtxm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/glvrvebua.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gfdkxyonf.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gzddkeodd.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gnrpocdtf.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gmjizzpwl.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gtsylbucl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gzllhvyuj.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gwbijsanw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gxdrabvbu.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gezvsuizc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/giuyxmeoz.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gtvxrxfbs.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gnhlxgwpv.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gvmecnlbg.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/goitktujj.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gbrtfamed.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gtvtqdyup.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gwcajxlyx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gvdjdufed.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/ghyfghrzu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gctczoxeg.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gsrvloitw.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gizikxinn.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/giqmzxjey.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gbayagwnl.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gtahvfocz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gyudxrfog.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gqugexmrp.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gbdqcoqaw.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gznpmrwgb.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gentmnlql.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gscywydlc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/grubswvff.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gzrldmbif.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gsdjegoee.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gfobudzml.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gtiojplzp.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gvyqrfiim.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gwlizhpmn.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/grpgsjivj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gmuissbkh.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gavzuqeqx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/githbqdtk.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gculahvzj.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gnvbpdxmx.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gdxvkapkg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/grabgtdje.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gfxpupzre.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/goadjgtxh.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gudhfypon.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gdnukebla.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmnwlapvc.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gnviywzlo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gucbjqurv.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gqcwobsfv.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/glykfuhri.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gswkjtizp.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gpbxabrax.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/goxbcufaz.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/glpgffqvd.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gfldpuzhg.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gsgnwfcgh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gjmmqneoj.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gquyqwbad.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gumsgyidn.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gzbwpuqrq.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gefmuekcy.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gytifgstw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gkjwbxwqk.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gbcnheiwt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gauhvsgwa.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/grvjerewf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gojficdre.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gvdznbkza.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gcfquiyap.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gawtfrbrj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gtzabwhid.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/grreenvih.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gdztttjic.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gdfzvstof.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gohlfpaxt.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gxxgmsdqg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gnonlqmkz.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gmeflqiio.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/grakhfjiu.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gucgohdhp.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gerqganyc.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gerlksxee.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gofjweimo.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/geyppvezp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gzcnjutgy.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gmlwviyzj.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gwskixgmp.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/glxpaaynv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gsisjxkfw.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gidjbrncl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/grpfvssyx.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gssjkbpxq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gxvibdpty.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gwcgsopcy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gnkzrrney.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/guicuicsn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gtkgchqll.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gkgunvhsi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gjjizxivm.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gbsjnumle.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gpmsydejt.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gnrsfazyg.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gokuxtbdv.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gtipgyvdx.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gwodzliya.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gjnaklcbs.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gkrgsuvut.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/glldburtl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gwbdtduqb.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gjkmjxhtd.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gqgtzxxtf.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/ggtkrybpd.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/goybefene.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsylwkmam.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gplohwwyp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gogllplky.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/glcugzgqy.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gqkmodkms.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gdmpwppyl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gbnltmifg.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gkvdmwgwv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/guxcqgeyp.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gbjaagvak.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gootjqaqv.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/giutihlxx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/grlrglsod.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gxjfbvhxs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gvyjiiczh.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gkivrymhi.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/grbigiogf.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gkwkwrfsc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gxgdmdvnc.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gbkdnmpap.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gzfwovbhj.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gomlhapko.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gdiaxifgg.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gzvnxmnpk.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gebuzxbcp.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/goyzehibl.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gfwugljzn.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/glpldxzpo.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/glayoobnk.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/ggdlrfplj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gwxwrkfcy.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gdcejwcnm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gcwiwpfij.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/getgcjdyr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gheuccrdl.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gplyvchey.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gkyogwqtl.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gtawvuxdb.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gnfhugqha.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/ghwhqwyfv.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gvpkxkuqy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gkkvaaifp.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gbfmvmuwr.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gbsdlwdwb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gllyuwstj.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gerlpbxaj.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gxvqwxfmv.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gsanqlfje.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gmuqyzvks.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gkrqesaia.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gqimmrtwm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gfvsobhgc.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gwwfdraai.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gctaahcjt.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gsepxkdjk.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/ghswvcjkg.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/grmppbehw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gwrwxwcqa.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/glbbtqbuk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gphvcngez.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/grpiufabr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gtncyzjxw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsvtleaih.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/guwpqkpsn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvynqupbl.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gvbjbpjax.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/ggyapvnir.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gjsdpgsrx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gahruofzl.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gdcjjgsll.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gthxqjtzz.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gbaklbmpf.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/girhvebhd.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gdlnxzkug.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gukxhuxcg.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gndmrfjbj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gdomqmlct.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gzgfvpfbm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gwrmmeozw.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gfqrzyxpl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gvtdsdrnf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtgkgaavp.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gfvigdnlp.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gldjrctlf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gbqmkmnen.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gbkgzydgv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gosjairkw.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gstfugcpy.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gnsndseiw.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gjzvbqphx.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gmacgltfu.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gwtpegwla.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gycvjyuef.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gyltcqgqo.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/guqeesxne.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/grgpqrpns.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gqercchyr.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/glqncuopk.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gbramqtep.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gbwbisiae.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gquhjjapf.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/geejbmngr.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/grxtmejrc.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gbigbnkam.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gfpduirqc.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gnlnzjcup.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/ghmnyekes.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gkcxiylxi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gbupseonx.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gvdkgisnq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gjrycbvic.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gdkdqigxn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfdsslcns.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gvfsdvrak.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gtsmbrppl.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gghobfndv.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gbiobgftf.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/grddstaho.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gnhlvthce.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gjewrijyk.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gepofawcs.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gtwplruas.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gjtlorwod.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gmjwqfqnz.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/glzbewwrb.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gzwwunhat.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gxmxnqxlq.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/glojnmfoc.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gdgiontbt.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gkzuusewy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gyffclmjx.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gaqhxwuon.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gmljkhsaf.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gztemfwdp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gqxjlwqvx.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gzdrrtahq.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gsklmqoll.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gquyfwpls.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gfcqbtbwa.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/guurqecoi.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gpxccjxhz.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gqtmhztnw.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gqgqdigrj.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/glcwteigi.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gronboxpd.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gbeasbkjp.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gqqzkywqn.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gbgyrlabf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gtdzziwyc.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gucrobzkx.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gyedbmdhb.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/glkknqley.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gkyyvopgu.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqrsiftvp.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gbobgaohx.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gbsajhozy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gatalqmck.sHtML


<!-- 参考信息 -->