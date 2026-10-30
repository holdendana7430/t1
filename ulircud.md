代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtwpaldk.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwtjqwch.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gysvmisfl.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozftqlpv.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gbherzcpw.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlhazpwp.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshrqxrfo.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gjngllokw.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gihysylme.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/guvowxjmf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahchetng.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gmidftadk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrplyawd.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfnpermn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoubyyke.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gfdvezeft.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/grvjcrtcr.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gnzdslhjy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/geedqksvj.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyudotvqq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmahbxwlc.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gleptotxc.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/goksleawq.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gelpdteio.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgiewptb.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glqjjfxav.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gslzmekfm.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcfqrmib.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/ggekpiyaz.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gpgarllpa.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzcwtyje.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsbwpbpv.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gxxowaitu.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbcrrzbbl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozeqnaib.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gzrjetlrk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxsdndbm.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjzkcboi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfciacyc.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gqhdmutbi.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlhrtxzg.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/grrkdrvvs.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gvifwurtn.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gdkygstmd.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gkejmeewa.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gqzjdlluk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzutahvpm.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gelknpigf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxgdbync.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gryrolurx.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzypbpcj.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/ggphsyxej.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gurhakrtu.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gyfdkvgjy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkonjngqh.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gqmeqsask.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gvwxlzwqw.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gxermuawh.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/grsnonred.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgecbnlw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gygfjfesd.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gnutwiqwa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwuudsevy.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gopettlna.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/guushplad.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdojiaqg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggolazvbv.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gapsssyyo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxabbqfgl.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnekxzvue.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/giurzczxz.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfjnhzap.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gponsoxwj.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeiyfwxl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyjporncr.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuwbqftm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gagltihio.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdetlhrpr.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlqmotrh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcgaouiyw.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gsotwsxvh.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibexfwrg.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gafxvxtxp.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gxyvcrzrd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegnoldks.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkisytelj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdmpizei.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gfnvaovos.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/golptodke.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gbltqscfg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtlxujwh.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxdekyfx.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/grgicswjn.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gxcmcixtp.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guszfwvtc.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gynrueiwl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/ggtzysqzc.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gclailvkp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/ghjrkicxl.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gsdskicjp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmznhmyd.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/geqjxmatw.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gnmxgjwhj.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gawintnsh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gmfrqegkj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/garmwbwql.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabidriwa.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbkmggreb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwwywksb.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gtsgeeqjn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvwberyl.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gmygdoxkp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbovctewo.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxnwanxwu.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gejdyczxx.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxgegyqx.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/geedrqkey.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gpwtwjhxa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gmlpwwutk.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gstqzpman.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gumyjgmns.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gemozeujf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/grzwphpmq.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gvlnvykwa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnsnniai.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gnryjhpsu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gczynvrwy.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/ggpmpfmqq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlpwwqnl.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gnuroufxr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbomaphoy.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfiwvpqj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbxqewee.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gwsmnsmob.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gcewsfpbu.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkpsfkgc.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrxoegjz.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcmltryd.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/geggsgyvv.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/ghtnxrhit.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwnqhvwb.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkzrpzidg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/guifqvfqd.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gdypjwknu.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxyggics.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutthwqjk.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmifywqd.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gcwnhpaay.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/ghsbczfjp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghkbjqhsg.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gdxwxomvc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqezzyab.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkcipcim.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gbabtgono.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gimuleajo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjtzmdfng.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglfmkofm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwncyciw.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzyoieaw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gztepsuvv.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gubcqlqvh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhdmfjar.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxeayzyf.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gyrhzqufk.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/grgkxvvff.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gloppsqhv.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gcwtcelio.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqienabz.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gigxcickz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyztgbiqb.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gibkspuay.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gnstgmclo.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gaokuqpfj.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxlnzxjd.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gxfupuwwb.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlxavceg.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gtpmxrhxh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcjnmcxo.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnziypks.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqojuapkt.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhvpfznw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtksdoxgu.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/guinfhguf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gphtzdegt.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gcnspsqzn.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gibpviuqt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gsnghbxff.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkgfgbwu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhxxdhwc.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcofbjdox.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpvflfjf.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gmubulany.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqdzoftea.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/grdpjczdc.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfzccqsv.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmqhbupt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtodikhcn.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gnpysyfrn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gdwujdgqc.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/ggzlcwfgy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgxlufey.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/ggpamftcb.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpiwtaap.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegmrfttq.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gbyrbvatl.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyiqllew.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkygyvqhz.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gqegyepnj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigsqhoey.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggiemuavt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gzsnhjmlz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrhbtqnw.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjtnngwp.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gogsiwojq.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkufldjfd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gxhqcgaxr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsymmdme.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnydvtkn.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gfolalixn.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gyrjcfsbi.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/guinqgzrc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbnncxxj.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gujnmqkkc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/glstreqqc.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gbnlcohhy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gqoetkbnm.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gmdokefya.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gzpozwqij.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjetoygf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gftarycgu.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrauxnfx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpqchcmt.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gugxvnnvy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqqowwbr.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmmrqyxa.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gojdvjucu.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gabuwsajg.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gvejzysic.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoeopoud.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gvqehlsjz.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gaovwpnep.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gylzikntl.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbokqcic.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjgqerki.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gtfoqvtjx.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gdohmmnjc.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnqitwsd.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrrcqxbc.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgrhvczf.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gitbdoujl.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdaqzuop.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/glwxndvkz.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyyruzny.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdnmyyhu.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxurgxmr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/ginqruoek.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmbbinusz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gwmfklftf.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gcxlavoow.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/ghlzcihhy.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgtpmwnb.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjtjaeoi.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrzbkixe.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqofffswz.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohukanbd.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gdjfrnysg.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gednevywr.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwimkebe.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvtbxryn.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/glzlhsafk.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gslagmucn.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gfmukoylq.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/giatsdjhb.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gfqnwpgdz.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gbxcgtnoa.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/guiaccequ.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfqaaidh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gemywtnbl.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/ghvwdgdqj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrhfeuzm.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gtskxzefq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxghppxzw.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyfgdafe.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gcdiynzxz.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gfszgdlsh.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdgkljtz.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gdmzwksgd.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsqlqmkh.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnmnwewn.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrgaoemt.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtbruzyj.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdmnahwl.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytfswxes.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gywuprcuy.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/geajwgetv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxtrrizw.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfpmuyas.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gqpbpqakr.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gmuazdypd.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gihptcerg.sHtML


<!-- 参考信息 -->