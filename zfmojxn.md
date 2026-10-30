代发 wailian999

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gqxggmjiw.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzsjmhxe.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprixxlzk.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/goxqqluwc.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gscbffdgr.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjthiwbpm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxayfyer.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gxdnxiwey.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gucfdoykw.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtagvknj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocblcexp.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gwsykehve.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswhdykkl.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugigtxyh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscxorcac.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gdgvpbbha.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/grhaarqki.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/glkashlcg.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gksaydthg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/guryxewrh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gbamhrolo.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqhzdcgw.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gmjayvbul.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gsdpwysiz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gcalhxlth.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gvlbchhuh.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/grfnaomke.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gadnrvvmt.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gzafpxexw.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnajznnbe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gjpgbmrkj.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/guczavhgx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gvlsmahys.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxcaauhp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwrcztbu.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyzmoupl.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gvncvisjp.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gerxpnjzh.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxdwsjnn.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gtvtrhnhh.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gppmubwje.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gkzkvffcz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gknloygez.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gwizwyxox.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gjnwrigbb.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpmzlulu.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyzpjklc.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gcxfynxan.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gsebcbrgh.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwvtvvwx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgfiuzoo.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gddyxtkmd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaqttemn.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/guqxuyded.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gcxhhqxxy.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/goaxdcpbk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gwstgeqin.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gqakorwpj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsjgmreyj.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/giuvbgvsq.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gkbutxlyi.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwppirsx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gogaxavdp.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcaxkmnxf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbbsanin.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyapvtaqw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfjoxlmo.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gfaftzmtl.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgmrmstz.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxevdseqp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnnhefbed.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gygrwkxjw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gitncxwwt.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhxvlqyp.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/grcfwcfwb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gddzkqrdt.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ggfvmmony.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbdjbzsql.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgblfwol.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/geulurteb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyojpdzx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqbhwyvq.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuassqqq.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gjuybcpxg.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuxcaknl.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gjheclkdh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqoxvenv.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpduhrzpr.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gtqazthxr.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gezoqlbsd.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gptbbfgae.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/ggalzxzfb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/giezbegfj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/geadjxjyu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/ghrrucxqh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvloywnec.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gyilaboji.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgxxdyzz.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfftmviyn.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzibyawhv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnahzadvg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gemcghjak.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/grcxykruh.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfighjql.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gjrbcnyjt.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giutfsrey.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/ggbngoded.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/goxinkysi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/guqclxrko.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gqpgveqbh.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/ghkjfwlfu.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjmdvrus.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbblefdji.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvgjljuh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryheklie.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gbaihnhvt.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gvkaumkzu.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ghegpwcrt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gpjazwyaw.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvfpdand.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnbklmqp.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxvdrrrr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcffmxbrj.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gfjjnujkn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfblzupxj.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gwczkamro.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gktiujovt.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gjjoztyiq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuikrtnm.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/ghisyzbag.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gukxiwggj.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvpnuhpj.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gyfxszqfo.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gvqguzsvm.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtashbdld.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gyudwtzoe.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/guzqpgkli.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghebpcjyp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gsziajstj.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbjtrjfi.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gisbjappb.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gffpgwapv.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/ggrrgnrhf.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gjhmcdahl.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gmkjxreqy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwhjdijne.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/ghmjoqvfx.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gdwsdypfm.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/getbxoycr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpiiupbbd.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/ggkblwxnb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gejmjsono.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gkepwqhdz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpauhfqvn.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzswcrvns.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gacxawcbf.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdsitmvm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuilspqb.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcdpqjnq.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/glaibdgyf.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gvvngsmtl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqbjfsbv.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gklefyxxb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gfbevbpad.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ganihswke.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/glduxbiut.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gskqoulrs.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxjinuud.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepyjkzbl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorhgyurm.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjnbvncj.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikhtlviu.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/grxcdpjuj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesgfgdrc.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpwizzuf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftpkjamo.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gqaihdhcv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbauqpvs.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gycidqwwx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gxdnhuhuf.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhodassv.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjtrltsc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gywxoiazh.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsbytxhz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gumqtldrd.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gyxtcfdzw.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtdhjheq.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpokjkof.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfbthnptr.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhdcygsf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsyqdime.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gnkeimovj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxxhiblg.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gxhufelkr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gsyjbyzdk.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweihhtan.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkkdnmtk.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnualpaez.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzdmvlnn.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfyucoho.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gngkpefzb.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbecxjff.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvkokkdu.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/grnwcvldf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwulbsgr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpelxchby.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpecqyamy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaohldat.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtypyuajc.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gsjyuzcxd.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gogvlmgse.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcgzufym.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gwanxphxg.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gywaaeglz.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gkdijzxzs.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/giwxxbltm.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkmpedhn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/grwvsgpuf.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gasumixij.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gefwqzntc.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gayaatuir.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gxnfhtvgu.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gwubordas.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaonshigl.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxtfmzywl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggavycllf.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxdxjjio.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwogzqfn.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gtskedlod.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsbowmhi.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiyeklde.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtkoqtkm.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gckkejtcj.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gygzoexjs.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gytaqceop.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gxlcyvokv.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/giitknsyr.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gpombprcp.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/grepzpxls.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gylcopjwu.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmopbqvx.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtabfkaaf.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gzsovxtlk.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuyfipah.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/ggttfngxp.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkakkaam.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvbbdvnt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gocgjlmgg.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipcnhqfx.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoiqdmmv.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhlpjnni.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gpuvcxkve.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjdxxmivn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqstdzdug.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkktxych.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/govszggjf.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtdqwray.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuaizkzs.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gotfvqfzz.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gfadmypdj.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gkicshsue.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/guokmnqjv.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gufwzhywm.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxhxcnwg.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvnrcmoy.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gbqzpaadh.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gxutqraal.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/grjgcvopd.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmebwbmmq.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgqmcity.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gezpdjvil.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gfklsfgyi.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkblnwhi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwxoypxh.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaocevem.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/glqipopyo.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnyhpqkn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/ggrpwyais.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gztfunyrf.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumtsdtjr.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuvzpsin.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvnmqysj.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyjqulfm.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gprcjhoef.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gkqvkthac.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gklcmptcp.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gwoireqzl.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gzxqvxzmj.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjkujhcc.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gqteqakoi.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsnjeusb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/glhyrjkct.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gapvzudgc.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gbqbaojkz.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyemijuaw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpolpbiin.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gvryfgmba.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsksargxl.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrqothhl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnszjjdv.sHtML


<!-- 参考信息 -->