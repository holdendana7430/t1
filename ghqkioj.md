代发 wailian999

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gctjxnanv.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gxfjjuifg.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gccgoglyf.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gtpjianvs.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfipeukz.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjlqefqm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gmotuvtpj.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydolawqu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glneehach.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gkbfnhgoi.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gawhufdoj.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gtamhknuf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrtyowsn.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/galfvwyqu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gftzatwij.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gumolhdne.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gbktgnlls.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gewwwtbnp.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghctlizck.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gcjhfszss.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gmspwwimh.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/goesorfcs.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gltwciogq.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfrutnjf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gtodorrml.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gldhylzez.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmdeuwif.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gzgftrymo.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gylrchqxc.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxedphdpt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvteklbbq.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gunahzqmp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbnovaoe.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccannzta.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gwjoncrwq.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtaumimu.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrmrqhdz.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtdemefdr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkngqrnf.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpmjsiyp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczizngwy.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdllonpu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyvjughl.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gjszybckw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gvyfhtske.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gidtftduq.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/grhgdtwgx.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfuqrzza.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gvyouiijx.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfrvjmbs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjaxvpqtu.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gjevcznob.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/geznmddwn.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvafwgei.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gjomtgriy.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gyyudczuu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzycixttg.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gacnewslk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrvrdjwh.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntrfijdr.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gltxzwfdg.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gvxklnznp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gturenbbs.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwctiamns.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfpvmvjj.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkbunrzvo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gawyymvns.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvfckvhx.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfpiezem.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gqayijwga.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/grkguyues.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gjceiqruj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grxbccdyy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/grerswlci.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjbnebec.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnysbsei.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gwwkdmatc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnbtdjlic.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonmplqhj.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayyqxnja.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhnpqklz.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gijrvvvym.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzajlfgwc.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gvrnmltim.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/glpohoder.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gukbtalmt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gysnqwpgd.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknprlvvb.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gugnkxkoq.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gmqdckyvu.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gfndfexjh.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gkztjolhz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gufajydgy.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gwfvxflxh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/goarupsjw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesfoadxr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gfvukvsfn.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqqmvrmb.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcqhoyeh.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gunuyugby.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gcummmqvx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gggcmwhtv.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeaxlufq.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gshomwcrm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhrgemxy.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntponesf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnosvvxyh.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvhkwvmx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvjijhdd.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gnehrvbcp.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqgrpqkl.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/grxrjkogd.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gvjcoqypr.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gjkkyfakv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbwhzvmx.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gciuxqfnq.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gvqyxenee.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfzaeyku.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedinkrki.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gagpifqfi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwhyvppt.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbmnezgf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnlwchzm.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/guhbynige.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoaukwnj.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gvsjkpjbv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gogpfpksk.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gouauhdha.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gounoqldq.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gsjtlctjg.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gpioxboar.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gwxkrumot.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwlsrqba.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcmbhdsz.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gfcpdowqg.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmciliux.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/grazqqcjs.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdasvmqpd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsuikixm.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gsabyxipg.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gizvwjpjn.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gerbskhsp.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfghnlkg.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqqtbbbn.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfxpufnt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqwpnfmsu.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjqrvdez.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gceropwnm.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gpmgtuqon.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gfhgsyvtg.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gyvntlcrd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbfnwhpni.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gazqdayza.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/grbampbde.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gfhrmzyzt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gyupqnpws.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/grrqgnbng.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkhrbuim.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gooawwcuz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkngjwet.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryfmssud.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrjtvlub.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gffltvfth.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgbewzri.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvbxaxavr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gwhudixvc.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxrnwnuf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfauitpe.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gzlawapfl.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gwsyottxd.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gfsbbnipg.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmqgduoa.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gpklfecac.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwftjsbo.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsgdaepo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrnimhqf.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gdbykcgdi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahpkyvce.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmsxujru.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuylqefq.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gbfwgbwzb.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclbjqogu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gsuienevx.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gauawkoyp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gwlmqxsyt.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/grlqzfptc.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdtxfrls.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gkxtzlgwa.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcbaomtqk.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gjhbxpxun.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/grwxrblrw.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/grycszevz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gjallkxlz.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gqbllevae.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gennyhhhb.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gwrkrlwbg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gykchpxaa.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gantjdvxm.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/ghdndlfxo.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gnvnsuwrh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyervegwp.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghamwocyo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/geaazclko.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gegcccyih.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/geutaarlp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxbtngzv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoxwrojz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/goimaidto.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhsdxpif.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvvxcudg.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gmobzyzcp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqlzukrv.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gizyjlkdb.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gtnvikkut.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/geethpvdh.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gvfmyjyxh.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjehiifd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gzlcgtnhk.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaeowpay.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfirlvgf.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gaivflzqw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiygjpyf.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/goghyugul.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaafvofwd.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/guflthknr.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/grrtxferi.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaskdito.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gzrnrlhjq.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glilelyxy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdcdaceb.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gcqskfezz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqbwgnpv.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gwntnquiy.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggovbjudp.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxvndibo.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymztpqob.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gbczrszvq.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gfwwjssst.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gyiqsipfz.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniawbjix.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxklpser.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqisyrjcq.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwjdpgvw.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvmlehpc.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/grqapvcxh.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gdlhrvuwe.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsykoylyv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gphvclbnt.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gtswrgimx.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzzfimce.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvbfjoug.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gorqwiree.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gseoylpdb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoleokxj.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gkmpeipms.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gkdhjyfpt.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gheizvkro.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gonwhcapl.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gefmrpinh.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gukqqljsi.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gorzgjurw.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbqygknk.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbtrkgoc.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gsopcxluk.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsxcbwih.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gqoqjscki.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzuldvrz.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gtphugaek.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gtfkyyixc.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gebrmslzw.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdbiflcar.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gmivubacb.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaaadkxp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoosbwmy.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvbzvdlq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gzufsofze.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gstgipnyu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqndmlkq.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmncgzza.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsnxfmts.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpyrmmfr.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtuqkndr.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrvfiuso.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/ghxzcztet.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpccwqfol.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmgjsqzd.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gudeykdhg.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbuuuhqi.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gyebmkzqm.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvdyrupn.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gyfntbhgf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gxbkynztj.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlokipgq.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjpfwudb.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gfhjkxypo.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwssktla.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gzssxbgko.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlavejss.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gdueknhpe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdffnfjyr.sHtML


<!-- 参考信息 -->