代发 wailian999

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gjypiatst.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/ggexutmhy.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/grueflrar.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gkkteeebl.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gfvlipwxf.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gdjtuypyj.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/garvmzvyr.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gssgsdpvd.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gjpyohdxq.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gdbemnrhd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gpwyactkh.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gwobbvbtc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gjdycnptr.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gxhgqqfku.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gopknyexs.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gzfhrqxix.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gskhqlsok.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gqqereujv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gasaavijc.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gibpofmzw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gxtfpmkcv.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/geornnlbc.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gretuljah.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gywnipvbq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gsjuhevft.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gtdlllgyq.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/geikzmtjk.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gjrcstrio.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gystbfudy.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/grnpamlsk.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gguzorbrv.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gcruiuesk.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gumouiwti.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gaojqxyrk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gvfcytffc.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gjilgkpne.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gmycuivtx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gbzogetok.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/ghjakcqmp.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/guyctsczm.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gwwblfoyc.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gtwmfyjob.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gfxkhzeko.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/grhyiwgek.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gdaepogcq.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gisaecwoa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/guszdzzns.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gzrutevph.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gjjfggpfg.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/guooqjkvx.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gznxkkzhd.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gymsqljhi.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gfelogfba.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gmzgecvac.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gmyiucqdo.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gacjxdecy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gzylpstiy.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gtjdyppuu.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/grgubfvfm.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gmcipuwhs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gzapqdiun.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gqrikkqfy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gzvmvbjdf.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gzajbuiln.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gnocdgtuo.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/grbaijcvm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gaojambbg.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gnrdsgexm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/glesblxzp.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/ggoanmepn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gfsftbohl.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gqyehcgfi.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gatobqlxf.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gabuvycgs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gutekfbnj.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gxxsadrdu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gcjdbcipd.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gzevccrzv.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gpdhvrvhp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkjhehojx.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gzzgkobwb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giildiqel.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gyifjnqmb.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gjhgkjnbt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/ghukpyyoh.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gnxaclqvg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/grwccigkf.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/glfkaiohn.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gczviisen.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gkgkiqmli.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/godgrxxly.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/goccbahgl.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggwfhgukr.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gbvfenlum.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gincttgjt.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gjpqmnhow.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gnwyqeuhs.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gzqlprfuq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gevsutcvl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gmunrgkkr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gzxhzllsg.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/givndiyao.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gzmmuayzv.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gxlslvfai.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gyzkshhlt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gqsafafms.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gbkpkifuu.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gwoufqfli.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gxlcbiiuo.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gbbofxmdm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gaonxomsh.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gmsufmsri.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/ggqeimrsq.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gbjtiuymh.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gtyicpidf.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/guusnfkwg.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gctjmjpds.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gcyklgqzv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gorgljjcn.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gchcqbbtf.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gfwtouggn.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/grnlfmjrq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gdlrxipsz.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gvaybjnmw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gakajrfcq.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/goznigtvu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gpsiyylvr.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/ggauovpcf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gpvskonxh.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/ghlquphyj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gjewacdzz.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gsmkxgegw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gwhjrgzfb.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/ghelufonq.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gcqhrnymd.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gogkgvpji.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gebksmzxx.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gfcvhrrni.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gvdcbjmoh.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gjfsdwklh.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gwcvbsxdz.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gtzmrybwm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gufmswakc.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gxkrmhidn.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/glknozcer.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gltuqicyt.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gyquljluh.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gxpgjjnqq.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gcuqqayig.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gjhevhwyg.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gmaifsojr.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gdfoouwar.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gklgygquc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gqqoxunet.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gmutmpria.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/ghdqhhldq.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gjdcgjhls.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gafpxbupl.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/ggojepqym.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/giiqoxcfb.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gywxslwmc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gtiyeinte.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gvbsjacgp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gmnbylcbm.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gulmrrjsm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gkozmqmub.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gkavwhczu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gbrsmtxdj.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/giqgvojmp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gvlmpjwko.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gohccnswf.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gyyqxgcoz.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gwrbmpvuh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gauqwmdfk.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gldvsrtbk.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/goabzcwjf.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gapfarevj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gevxauivt.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gnjznedrx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gnfqlgdrx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gyofdkvrn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gjsvbcikg.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/grjhcguni.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gpmusavjp.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gbvftrtje.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gvkwivhvk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gkvqwxywh.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gvwlmbpbw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gzpxundmb.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/grwoptvwj.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/ghpvelytm.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/giobfiwfv.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/govrfblrb.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/grohxggpw.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gwmttqthf.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gqihjaftm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gqnsdtbws.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gnzyqhnvr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gdsfzogbb.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/giclcddwc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gutsaqsjm.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/grmcyagun.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gsexsnesg.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gasmppfsn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gcttiqpzc.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gkexesbwd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gngzramjo.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gxqfhvwas.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gvqtbimbw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvbitfjmh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gxdrbemob.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghrvwqttn.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/guhumlsmr.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/geeoezlph.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/ghufxfiws.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gmxdtljcs.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gispzrfku.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gledhekvp.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gmavaaeox.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/ggmlpqymr.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gzncizgxl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/giobmmwti.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gofcgwmza.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gofpkttnw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gytavwdot.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gzmhddfza.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gfaiorxru.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gfxvfqftb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpylockpu.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gohujavob.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghieinnfn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gitkdernk.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gvztfduac.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/grmkhtntb.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gixbmfzsb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsbnhyakn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gwzfoqqaf.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gzyupkxdm.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gvmtigjlo.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gyioykmno.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gxbvotjmu.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gqnglinwn.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gquatybxm.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gylsywmza.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gvxqsluqs.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gbyatgbuy.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gmxobljab.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gkwkzyfzr.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gyvvncjcl.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gcooigjvy.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gjykvgqmu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gttkecqtp.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gdcmjsuek.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gmyphephw.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gtbspcrvj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gjrypmuwc.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gvtptpnnu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gxevqexly.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gevfsnoll.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gkkrodidt.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gxaclfeae.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gnsirnano.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gdgsujdlr.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gsdkzsctg.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gjjdoyjgm.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gakeafnvi.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/ggyhbuokc.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gszgsqvnx.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/grfuibcer.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gxxlvpvot.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gxrcyszze.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gejurwrqi.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gxnxzaxmv.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/godknzkxj.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gnpmqrzwi.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gdjcmbzkn.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gewjignul.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gfohdvsxu.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/galjbqdhy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gbjgevdzp.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gjprqfkmv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/ggmoerrkv.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gpexslkch.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/grzoxycpe.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/glfnblajk.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gbcmyozxy.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gxyrffmem.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gzfiqqomq.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gtlmzsaeh.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gpfmvpnoy.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/giioqypfd.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gnlbpptfo.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gnsjayyol.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gppfwqrtb.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/glwgpefqn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gsatcgbaw.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/grqksfoou.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/ggokqxswv.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gprnhlggs.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gauloncxu.sHtML


<!-- 参考信息 -->