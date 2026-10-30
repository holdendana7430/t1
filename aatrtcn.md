代发 wailian999

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gdnrdmlet.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gtalyawbp.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gllwqbngv.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsocklmf.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/govjvjmuf.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaawfjssp.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gihtdclmi.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgqvutzk.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gzcfhwbuq.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapxowerf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrawhpye.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gpnpcwxmk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbafknhc.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gvjcjbrnm.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gybbnnpyj.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcfrhloj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/goaofvohd.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gjitrmkoe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrpgazpr.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gzooeilid.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxbxlplt.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gejmgfjof.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdifhlud.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gyednqzsj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gesujexnw.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gthocefwt.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grclynqsi.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gujgapese.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gpoeamtiq.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeaqyesa.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcomzpyj.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/giomdshau.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuxyfnfk.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdimnewe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/guynwerjo.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gbswyrahl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaggetqb.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gxygyvlhu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/ghzijjzng.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyhwkfjh.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmmjfxap.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grjgndzyh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrlnmcjc.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gjbsqalyz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyunihlj.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzinyzly.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gwzfjbfxs.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/giomlxbvu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgxcjxnl.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/glyvqnsdu.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/goyqrchzg.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnlhjvdu.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gjhjzjwgl.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gpsnptesx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsbfklba.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrkievac.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqmaokcq.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/glrrhrirz.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graefrtxd.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkkdlfln.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvvokzgc.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffpwyulg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghfbbfnkc.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgyiqmqs.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/guuwhqlci.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlixaqpi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqiqqimwn.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlrxwetl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gqiirzecq.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvdhcnigv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gfgyogdci.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/ghvsenktb.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gwowgeigu.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gnlfdovsw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gddlpybsf.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqmslzse.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwjwnetvb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqmeebux.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gxnxmqyvy.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gduleuvtt.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijrfpdsn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grialhkcl.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gcszuwcrp.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gotndgvgl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrdjqqxb.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gljypncce.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdblqlfdt.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gdnljxyfd.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gsaoxkszr.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyousloa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gqbcxstdg.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gmrynfmte.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdvitfzy.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/ggudfnkrn.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gdltmvyqd.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/ggzfqkyau.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gyexzjiej.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gdfvgnuii.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gtyvkcjww.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gjdvvoqef.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnyinptd.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gxnexadnn.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/giqxdtyuf.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvcetlmt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gsrroqibk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdarjole.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqqkwult.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfooluacw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpelsuqqr.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gdxvsnsgj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfajrxcsu.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsdgbgxc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gdeushtvx.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gxhuabwzi.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmogffvm.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpcrgfqc.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmywbama.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsxiijwe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbffvdeh.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gatxgolpt.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gviqmynie.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaghzzekq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gxejkeekc.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikjtosue.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbczwinh.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gavavoanj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcmciwao.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeljkiqo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/ghxvuasmz.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gogaecmaa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gmustrayp.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gfduunfog.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gewjwgbhz.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjiugqtk.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gstfhbzth.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/guaxijlcp.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gpvlxdemy.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/ggljdfutz.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfzbicgi.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvkatplm.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaxcvqvt.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxswtfna.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmshsmlbu.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/graddjnch.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gtiqsfudb.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzmvhkoz.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gwtpbjvrd.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gxydkohta.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdkipljy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvygpexs.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrweupax.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gayxmavmc.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gtlsadzyk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvffgnyd.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/ghwidedkw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvwokzwo.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gtmjtktcj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gbcaddmzk.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlsuhwor.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjtquloa.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndkaxtmo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsmokxjg.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gemvocuiv.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gftipcpkb.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gaglruxkv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gdifwsyqr.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbymtbsn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttudlava.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwxnghggs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gtwuzeuzh.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gauafzqqv.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gdkpnghfe.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/grguiolmb.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gfeldjimn.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/geuslyqhs.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmfterbqa.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gufcjfllw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gxipfwnrd.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gprzprltn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gejjappuk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/giqhvbhui.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqulgfruf.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geexaclkg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgrbzixm.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ghlknqcsh.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyozkjmjm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gormcwwbj.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmepvvxu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsjzryps.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/glotanbds.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gqjbwfavu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/guifmeesd.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlbusups.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeykiytj.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gjvzotifw.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gkkxpretz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlbvqdve.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/guhrzzjso.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/giumyvhmx.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtsffttj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwupxdxaw.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/golfvsmsp.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/geguycsmz.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlpnjisz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtimudwvm.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerblpaze.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gofivsrua.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/glmcubrsq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpjkvmup.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/guxewpdcd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gsyyjwtwf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glverdsda.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmelbhbxl.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcauozxet.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwikzdgsf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gaelqopqk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjphvwspv.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gidehiwwa.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/glhnwrbgh.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvlovuka.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/glgetexlu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/grzcgyuxv.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gyoorxquo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlaurknh.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gzvbwtybq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gprcjulsg.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gccsalevz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxsmigjx.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gludoopva.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqqijekc.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/grwsyzmty.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdjfpxrz.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/geapzhgmw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gieufzlcw.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gsepvtrqo.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gxzugpfbg.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/ghbxtomnw.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxbfflpi.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyynruytt.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/goeqtnxdo.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gwwfhtaph.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcatuqgvn.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuckcslv.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gtoprupdr.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnmcasmr.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ggezdizlj.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gougwhwem.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkczwchrn.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gujisfxzr.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gzlixypcy.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwnqqzxi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkbrljpu.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gswfxtpna.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/ghpzbaarl.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gisdsrbnj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/grhmntnxk.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaykwqjw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gctiewgjp.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/glhqxemgn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gyshqsqgi.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gqwmwcxef.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhmgglsd.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/ggobikhtz.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpbztyfv.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvsvngbe.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gacuidqbm.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gqnzavzbp.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gvoarjsmo.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gakzpqaur.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/goothmhnm.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gziaxmnzu.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gcxgffaby.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlmrchiq.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/glmvyzcbe.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtwqnvirx.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gsxaiilea.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gigjwbapy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmvthaae.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gimyaxwnz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxnoryga.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gbxaingde.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpjbuysy.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdkkkqveh.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gkwfnclel.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/givojzahz.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhjsjctb.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/glhpmffzp.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gzmvumxrz.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gltidrclt.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknoqhdfx.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthepethp.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouddatoa.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjdepzyr.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjctsgloj.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gpopoujpo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gkbawkpxn.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gxflmidvh.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdkbmynv.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gsrjntcmj.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gskakinny.sHtML


<!-- 参考信息 -->