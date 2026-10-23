代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3xxydbimc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3szkuiibo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3cdacaccg.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3cfanbewl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ymfrozou.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3pcuqerfu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3gllbslxm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3sqvowxlm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bvsqkqpo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3tzbjptdk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3wvzhaszu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3eykbwvfh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3uyhhyqoe.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3xmltobaj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3znunznls.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3potxapxy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3jbwjtblv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ykfcvgnw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3mwmvsbql.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3xfzirjzo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3agzgcnbg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3bhgnrjay.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3thlvgolj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3tvciceyw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mwlaxnyi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3gwmhirew.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3crrktvha.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3fdrypoij.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3kumrwagl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ytspmtmn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vmjhkuie.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3xyhsrjlt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3wzivqdyf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3uqrrltvx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cxiemhwy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3fzpsggfl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qdmtauty.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vpgtlcgn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3tkfqooqq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3kpxqjvvt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3hzdgawzt.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vabivuka.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3lksfdhin.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3llzfwcwd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ekbaeodt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3rtergzif.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3qfincuel.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nmrfxfwi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ylpencil.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rluzbmzw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3fbpteflv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ggagylwc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dxdexsss.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wodtcnkd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nazrlywi.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ovuytxwi.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3oebkjikp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3bbhovwhc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3leeedswp.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3neewbkaa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3nkdkewsx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3lklayzrn.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3azgpmvdr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3msaxtbtr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3trpiwnvq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3fcahclct.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3qrxntmrv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3upesrekx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3hfaukrtr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3kfukoqzw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3rvornxdm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3driqchhk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ioxeecha.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qoynhloo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hdzhhxkj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3fcfetkeu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3waeqzrjd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3spgaasxb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ebhbwywe.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3mlwljphd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xjkpdejn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxpqwxln.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qprmiijd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3xgefbjwb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3wykiczuk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3fahjrqlv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3dcsawqeb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3dgfysmav.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3njzpmsxx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3qezxtocz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3nqixvwtm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygbgrtwg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3skcgasep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kszkwkdz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dpqeyfpk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3icaoqusa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ybdfclei.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zwavaemt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3uuxcgesj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3rbfwngyt.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3spteoobh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3tcouupek.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vjnnwpiy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jgrpyvyo.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ypifuvbz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3drhqchjt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ibvmgbzd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3mfnjjwax.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3jhqtzrrl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3tzcprmgd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3wnnadxbw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3rertaloj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3hyfxzhhj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3pavvjxvg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3oxyvmkyb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bzqqklfd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xtdemoes.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yqhxpwur.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mtuoevof.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3emmnzrii.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xzfbwmpm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3cwuwvhjr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ntjyjric.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3kzkpuipw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3fmoznksh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3lyuquqti.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3adtrmdhw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3vdmcnxek.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iuzozaeb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dlygxchc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3hgoxwzng.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dksmyqlx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ybdfoasr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3quczevcq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qexbanjy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3qxlzhskp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rwicslla.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3mvlkllcm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3csqbeuil.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3lcueyzpw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3lczifvex.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3gxywpnid.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3cfdyldzw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3zqcnngnu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3pkeyxtby.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3syjvhvog.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3hcvjdfcb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ddaelsjc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mjwplssd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3aqhdqjhh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tuphomgn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ynjuwbny.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ymxpoyel.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3fowyjatj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jgnfwykm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3afnpgtnu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yxghvbpq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3eevxhghw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3lpgzuags.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nilxjquo.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3plavfvjz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3quarmlsh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nftzskxr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3emqkwdil.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3asviscwi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3cwgosulq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3vjanadmu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3krrusvna.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3nvlsjvol.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bockluut.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3dmfgagne.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gfapnvfq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ejoeuojj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3loubwbny.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3kljfders.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ajxjrrsx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3oanhfdpi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hdhoqxyi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3hjreqaaj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dthrmlgx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ohjusgnz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3zhfjozzh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ijxxewuq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3bwbxtbbn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ryivjlrx.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3rhcpjzvh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3kmjsuizj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3icuocumb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nzcrxhhg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3zmztcgte.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rqkvpsnb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3eswulvpr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3axesqyhb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3pffcrsdu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lzqvbfzx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3fpaamlfg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hwkvqdra.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3pxcwnivk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rwieeigw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3rsnceoho.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ubeovkes.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tztocduk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3fvhsuotk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3fvgadbzz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3cgzdodjz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3drtzuovy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3dhqxjqoy.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ixevgwjc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nsnkpzlz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3utxfipik.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yjhrvrbt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3znayeydf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdwhfziz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3klyncqem.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qrlynbas.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3khflcnem.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ukuzvsrq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3hhcanpik.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3lfblpmbp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pcxawkuo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dqovaipu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvzthdcu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3cxcnpvvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exjngkgn.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pfcdhiga.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gxwbgacm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3sllyjbry.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3dthcogwl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3yrebcgtu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qzrwppvj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3lhhotxwo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3vijbdjso.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3soskgjac.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3hvlxejzv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vogsurtc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3smeoafru.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3geamhyxt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yijtfahm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3snswmkkb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ajbugkez.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3qxumkskj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3rpdgbrjq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cawuddon.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3aypycrbd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3iwdziadn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ivwgqxkr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3rfgkndus.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3llmvafms.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wvfsoirz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xohodvzb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yrocsntx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3eaaayhql.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3uzgjymfv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zblsdgya.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hyqgjiua.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3safoithd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3avxmrvff.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3wavuqqhp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ylmrzuks.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3adkbeobj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zpypuaqk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3rdqideqt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3lmkigwlx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3shvgjaqg.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tjjamyxx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3cgofejqm.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3zsvznypd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pvosnjrl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zrcqxpvq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3xvdgnmlc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3cavklynm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bgzkhsqx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hyxuslrw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dvvfqqgd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3lqioiclt.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xdmfyctt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3pdtbscwb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3cnbbmlpc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mbfsrmwk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ztkogpte.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ovsloypt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rhqgagif.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3nbqseqxu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3cmtyfvur.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3csmpignu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3blzvpolr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3beyjjuun.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3krtyrnxb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3dtwmwijl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3mvkfxoki.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3pgirrlob.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3vnnkjjhh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3bawpmtqo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zpkexzth.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zqvvpgdb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3cjdtqvql.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3owxkkwlk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3tdqyfaoq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ndnkkhzb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3idpftkre.html


<!-- 参考信息 -->