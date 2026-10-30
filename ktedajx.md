代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gzxyplrfb.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gjkojuagh.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gsgruymfj.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gcjmdottc.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/ghdxhhspu.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gmozjqder.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gdkucbgps.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gsmddnjgj.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gfbmbhage.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gujoosjpz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gedxxowvr.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gxjyfjunr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gjaitmkhk.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gmbozpyok.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gtqseraou.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gaoxnaiex.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gjhuhzggs.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gvrmlrhin.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gbjtbqclk.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gdflrystt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gfksitesp.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gnvsysiak.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gpmsxutli.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gkxgmogqx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/grxvehwib.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gufnyaxgf.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/guwualtwd.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gzuhbtqfl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gepqrbciz.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gqolctxzz.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gurxegiey.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gohqsaush.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gjktxarwz.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gzcqkbxin.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gdbqaaqop.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gqfiffzck.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gpplyhyzf.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gculelafv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gonuevixx.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gqpqnhbxr.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/ghljeczhg.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gflmembnb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gyawwurjk.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/ghlhdzvkn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gtjnkxizt.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gclcsmsmu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gueriquth.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gwtnnmawr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gsuvjcgae.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gghjmoxlt.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gfzjkbdrl.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gpybewhaw.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gbikjpbmm.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gerljmoia.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gkgsqknuf.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gbvhjhbbi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gjfcnqtrl.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gmidnvzsg.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/glzrpxbba.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/grltypfhd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gnlibqbqt.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gurmvxlyd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gtlhjoxzc.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gmyxqesor.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gsogrmqci.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gunwaqakg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gtdwylwsf.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gvragcygp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gdqzbnuvv.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/ggtnppndx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/ghrojqjfd.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gsuerofxd.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gtqosfyeh.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gdqucjetv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gfyedesdh.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gditslexe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/ghglgtxoz.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gqrgzcivk.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gdhmlbzew.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvntqckcb.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gqrxfmeua.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpvvkbbnb.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ggffldoun.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gliytixud.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gxtknlmde.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gvjfprslc.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gburbfkbi.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gapogsufl.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gckkmhjym.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gbqagmeyq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gqvjdjktp.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/geddpuoql.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gfyhfevep.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gelrvvkyt.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/ggcqpvfqx.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gqyplhzkv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gknljyapq.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gfwlohcvb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/ghjyjxmxg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gkxrsyyum.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gprkkuktk.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gjzppelkj.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/ggjlnkxix.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gcldroiku.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/ghynmnwrh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gjkqqplam.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gzanbrlcj.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gdibzkdbr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/glhfdinah.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gjwciuxwh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gckbgrtvv.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gblewizgk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gbgzshxft.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gjouspzfp.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gmykcfurz.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/girxojarm.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gzgcfzxht.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gtzwrigpa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gmdumqwxt.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gbvpzraol.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gnsrrwhia.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gboxdxbcf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/ghvugshnz.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gkggjswhq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/glvdveuhs.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gfjywqdfv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gdlcnrwpx.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gjwgfmkzi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/ggvteuctq.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gtjytrgyj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gsnuaebyo.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gwtiqzgqu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/ggesmylxh.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gcjcvkxdu.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gvllaqjny.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gqhtfrghg.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/ghnrazkzz.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gnpnztipi.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gilpajqhm.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gqerzbidj.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gdwchivcj.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gnzlnquzo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gffluadif.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/ggpuzuyff.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/ggduwpqbf.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gzaoulczi.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/guguozueq.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gpjjhewba.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/grawxapsu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gpznlzcyq.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gxvpmlqbs.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gfpfhopta.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gvejujfhm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gamrhriaa.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/grkirlmns.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gswexxlub.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gtkbbepma.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gpnqrhqmm.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/ggjrbmxtk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gzvipenpg.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gnmiuuioy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/glfrzcmcg.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gjfvvczix.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gsrvfudpw.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gzofznsar.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gfupyclgs.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gzedmiurg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/geilkfsaw.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gaopqnkpq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gjznvncdy.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gzbdievvt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gzqepcccc.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gposqpadi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/glqjyjyfk.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/ghzbxukyh.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/ggiciorso.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gnomrsrdt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gssyfcitb.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gujyyglcd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gtzawpjrk.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gklfqdjwn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gfvpjhkwo.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/givvdvjor.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gtpkzcqqz.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gqubqvuul.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gjoxivkxy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/ggldciyhg.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gmevgzofb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gdwejcrqd.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gbblolnbi.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gxuvctrch.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/guhlgbayu.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gdnedagid.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gvfetkfbb.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/ggovcjbib.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gzgguharf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/geromhwgw.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gdymqofdr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/ggmpvanlz.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gsxuhzjcn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gurrkymtd.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gyxabykut.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gmojoabqk.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gzhhbipgm.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gyhsvlait.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gqqwjbfmi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/grbfcxpoz.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gwwlhiljv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gvjsgnmdr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkmdskrlt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gdsrdsydd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkydprylf.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gliwmdiix.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gzhzubckc.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gjvyrcmhn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gsxvidevw.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gqblglgtv.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gmloyhfyj.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gautiudow.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gcrbyxacd.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gvvaebxvo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gdaaraykp.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gtajakvah.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gpndgvhju.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gzddazygc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gznzrzobr.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gypznwkid.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gymsvabgy.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/grvhutzlq.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gyzpodvic.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/govoxnash.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/ggceacakr.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/grwdbrqfo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gzaeyjvpp.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/goydqpegi.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gkuohcpau.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gdtwwoagf.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gwhqpthve.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/ggdskovjw.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gqxyvyzux.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gcdievjzw.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gshsonmpt.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gjhalkxko.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gpodedwjg.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gsoesibxs.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gbuwebfyt.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gmytkgdvr.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/glvllsqvl.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gvozavlbq.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/glyxtadmi.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gtjrznbxa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gobzqevlg.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gmxsjdogy.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/glemkeeqn.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/ggakibgfy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gitugvlvi.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gdqfxvebu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gntupxgjo.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gpacoaaqp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/ghdhzrjni.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gsskwogai.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gttdnqaba.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gkysbnomi.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gkshundwu.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/guqrdlybi.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gkvlggaby.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/grzjdrnou.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/ghwiwnybm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gwykizjlh.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gtfexbkpd.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gvjbnwlez.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gnjgwimrf.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gfinvojct.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gfrenatby.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/guovpdkia.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gadhjpctf.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gnjhqlwdo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gacgkpszh.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gebpxylmo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gahnurppr.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/glkmsznjn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/ggldpfeqf.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gerococjl.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gakxbrjam.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/garufhtie.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gcpcqxmhm.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gjtmavwrw.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gkkisdjln.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gpylpynwn.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gouisbhul.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gqvjqwdmr.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gvnihoylg.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gjhzzlwqr.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gmdbveovc.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gxgbfzldj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gefwodzjk.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gzejrxwot.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gdbiwzjiz.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gidxftkme.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gfsbhowus.sHtML


<!-- 参考信息 -->