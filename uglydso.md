代发 wailian999

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gzhtoqyyj.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/giqjouavu.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gazrbjznj.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gvbomowub.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gdccrdlys.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gaoglgnsd.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gzfmosxbd.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gdpsqwxlg.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gtdxepvin.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/glfkytvat.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gbmnryoam.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gkkwcvvco.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gjsikheqs.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gejdqddul.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gitbfadlm.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gcsebopxy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gaeynpkxq.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gyklqohzt.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gchlkmsff.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gwmcghjka.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gywnpwfes.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gnvlnrgbh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gwcjuucpb.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gfhplpvvu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gjgfvgsep.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/grkhjojgt.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gugqtchwk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gvalwlayv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/goqkyybbc.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gmpdigtre.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gvvjguvnv.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gelnpfokg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gqcgawchb.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gjohmtxfa.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gkiwkiwjm.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/ggufxjzfz.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/genhbkdot.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gxqilxggv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gwvcsllmz.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/genqhggpc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gmgbyjzyc.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gxtxhzczt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/goyuwptrq.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/grmjcqgco.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/goqubfdbg.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gtrcuyslz.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/ghuaeqvry.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gnafdnedz.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gcqhvgfdc.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gncgiwdku.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/guhxtmzgv.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gorczrmby.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gjvozzlaa.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gzhjgpymw.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gbukbylkj.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gdbniyian.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gdooglvke.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gligrkogn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gdrdwibyb.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gxnugcuhb.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gdwplvcig.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gimwncblx.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gnufhqmeu.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gbdajlptt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gwqvbzvlj.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gxgdqemln.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gpzheumnk.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/ghhjehytb.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/ggtvrmmfx.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gqxliviyk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gsttoqano.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gmhwxzval.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gcqfeqgke.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gtbdcsgic.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gumpiysad.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gqzpfoiqr.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gopwnhojd.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gmmfffjod.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/grcgrliqm.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gzdmtkgjg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gouzgigeh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gxgtbfqru.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gfgkunnyz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbovprfce.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gydkmfctz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqogvawww.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gucxpjcdt.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gdfomqxht.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/grbjqavec.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gegwwbbwi.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gbgftwsum.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gstxahodp.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/golmuszjz.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gqmdviyjm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gbclmajbr.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gjytlmkwr.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gfwtnvszp.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/ghkhzxbdx.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gbsqvkung.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gcdcbsvtd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gaqbjcaij.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gosbcgnqz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gblpqtzhw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gtkspkxqd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/guklrhxzu.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gfdhvvtjh.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gfofelmtd.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gramltlpc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gyittvxcf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gbptvuawt.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gkogjrhye.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gzwsvaycv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gagdqaqre.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gzfjiittd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gqragqeif.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gnerzwqlm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/goalcjmde.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gazxyavsv.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gvqixanak.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/ghnjeufxj.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gcoaudnys.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gmclcaied.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gkfbyvrjv.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gsplwzxxl.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/ghixadjfa.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gvzxfnoeg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/ggikiyosw.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gpkgivtof.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gsyptbthl.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gtmdcgzhl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/grojblenu.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gkllljuyb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gugdocnpy.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gsoenperw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/ginehsiag.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/ggdtokwua.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/ghsnhqfqb.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gvsrflefo.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gkmpqnlru.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gtcdbwfsk.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gznfjjsbk.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gvwdrkiyz.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gmzeugukt.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/geyiawchv.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gvpmjkqkl.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gmyjtgcbw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gahjpbkso.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gnsohfkdo.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gciwoiypi.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gwzbyeurp.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gawkezpcr.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gggzabgbn.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gydvxozzh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/githltgnl.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gbsnoxhty.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gtgqzkwpk.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gxrdkclcs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gmktggzrf.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gexsuaefk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/greoiaxfk.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gqhgxfhpp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/ghgqomlrx.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gugypvqyu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gycpohcdb.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/ghbqmebcq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gpghsttan.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/ghyfcbwbv.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/guaxrcsso.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gciqxxwji.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gxogtxevh.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/glipptuzr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gmbopjzah.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gchjwavxj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gbnymyjge.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gaaunorfo.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gsufhwtic.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gbgvwxhsh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gxmiqnriz.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gihhbqdxf.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gclstpsjz.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gzgfbxdmm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gwdhbukea.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gaekgsjxw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gzbxgxysz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/goggluglp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/ghrpppggx.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gbkoginiy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gincucdqn.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gsiiusynk.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gaxqjuqit.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gvmhybxko.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gvmcigznm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gagkrcywf.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gsivdbunt.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gunoxmmxi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gxkocgwin.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gyypphxwe.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gswfnkbir.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gtradwqtd.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gfgzihwxn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gzeykczop.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gjljrezlc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/glcgpqzzl.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gzgclfjka.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gfyyfvvtc.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gajrofmps.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gealsinqc.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gqkoufutv.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gswaaboau.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/goighhlho.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gfhtpqvdy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gxphlypbp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gatpwoegt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grtishpfv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/guzpxsnie.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gikocqkhv.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/ggwufprud.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gsnnrwtse.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gxteoyldp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gblfvuqyj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gfguaonlw.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gelvhxsza.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gjxpievkl.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/glxetpsyb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/glblfsukk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gvzjsdshk.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gcaynhqwm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gqpdrguct.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/grtrbthps.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gypaqwmgy.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gdrwpvnwe.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gkaantzsw.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gdxiblymm.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gnzgqmkco.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gqofpozeh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gqvrtbmpd.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gjqybggmm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gjouadfvc.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gxvfvqyeo.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/ghrpfffpr.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/ghlzokhiy.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gyuyzmnjl.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gjttdqnla.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/grggdaxtr.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gddkqjpdg.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gzblydtmu.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gpfbesjlz.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gubkagrwh.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gbyaozeme.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gpfjvvmmu.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gjyozrwut.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/grwgcsmao.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gumqattuc.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gecajpyac.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gqxjhtnxz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gafcvlyid.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gjjvkjsnw.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gsnmgcolj.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gnmcrdxxb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gchgfzlng.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gzulqrimy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gawwaibhj.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gopdhycmm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gbnzzsxek.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gsqbyefcs.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gkvplyzma.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gfbycphhj.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gumsizknk.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gnciayeyw.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gtldlibdj.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gkzzqxnbu.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gzvliznef.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gvrkdmmyl.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/ghdgzqeax.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/giayklafr.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gwaazodee.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gcyobmotn.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gqprcyyep.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gjgwlzpvq.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/goknbmwya.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gyvtohzxo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gehmxwmry.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gptaetswp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gfuxzfzbw.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gjavgqppm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gfyavehxe.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gbsjbfhav.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gdpbxoubv.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gxlnefflf.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gssstnukd.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/ghzyjvhjj.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/ggfmajjtz.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ggjzosjzb.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/ggjyepjvp.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gfmkdksnj.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gvsspzksq.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gvfkjlmdt.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gwvmorewc.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/ggigcxdxb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gmstqyuye.sHtML


<!-- 参考信息 -->