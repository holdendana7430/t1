代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/ggurbsobc.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/goqkczqzb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gckehyhyc.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gjjqdorhx.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/ggslenjsi.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gxbgzqltc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gwtriqkfp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gygmjtnra.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gkvffbkui.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gdvzohvlg.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/glxrqxfpg.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/glaqnjwuu.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gexcjhitp.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gcufjkioq.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmcvgdlkv.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gqonjwmqt.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gisxlptdw.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gergvvldx.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/giwceppgv.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gyxclpcwp.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/geaddjlvq.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gdbezogvk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gvapfrzjz.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gqtaiwwtp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gcjdtfgnd.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gmfsaboah.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gaizjbhyg.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gqkgmrdwh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gltyrtroy.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gxifcrfqm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/geidfoobm.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gmasppxki.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gudmjywsd.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gqhafjcpn.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gdsiysnjj.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gqnlqxhqs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gxjunxbbg.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gmoansdzc.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/geypordgd.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gwumpyaoa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/ginqpypmx.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gfacjtvav.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gwcyghgro.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gygmhfwxt.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gpwvxewnf.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gfwcuyujy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gbpqygaky.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gohqhejhx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gidhvitea.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gqjdkwsbl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gdndwfdzm.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gwjylvffe.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/ghuhwlfeq.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gvebydymn.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gkphlovvt.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gbxbahtjd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gzbamdsqg.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/glnzeunje.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/ggvsrkicv.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gpdyqezec.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gaejtgiee.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gjwqapkuw.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/guniputnn.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/givwhgdlb.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/geajvnnqi.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/ginbhlhxq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdlujyyue.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gsfsccwvb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gagqhqjrj.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gbqyogolc.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gernyqpnm.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/grnsrrifd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gammcecib.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gxrdpaurn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gsjptqimg.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gbkywqsrf.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/giohaonpr.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gkuzbnepk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gchxixkqy.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gjzdobwcw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gbuqsdsge.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gnsudgqry.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gsceahgli.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gqsgmvhjo.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gjfkgrcmx.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gsezuvutl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gvplxlmww.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gflxuqfyt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gcnwijhlo.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gocpxeukv.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gaepjdqgf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gycgobxbj.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gfiwuiukp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmfiyxeok.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/grtwtoxby.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gbpwknfnr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gqcuoigws.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/geuchruav.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/guauxyygr.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gimirrkbu.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/giqhcsghh.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gaapiqgsi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gaccbnrdy.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/glasdbvcs.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gqpdpytgv.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gfokegiju.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gbzbaojpt.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gkiztluvv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gdzwmuddn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gsqhgjzae.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/grpkhlykj.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gaekjirin.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/guafbnkbd.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gelbozail.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gegvwipzh.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/goshgxygg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/ggwlosnmm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gdlbhzeki.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/ggbecpsjt.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gogqxserd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gplskqtho.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gvlebwxdi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gxsxdwnfz.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/ggmrrakjz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gvcsoykil.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gmuhawcxl.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gqkcygquc.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gtnrqvinp.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gfwkzchfb.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gpwwjuwbs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gecqwalwc.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gyqyolkbc.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gxvqtcfew.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gncbzgefy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gbfjdyxdp.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gihudzljs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gtxmdwxnx.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/ghkzpiwrv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gvbdrqgme.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gotwrvcqw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gnhxcqunp.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gicfwguoz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gxgpkrdgj.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gxajrdsaw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gbfvtxwht.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gflrnijvm.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gedinajwx.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gkgousyyr.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gimrltvol.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/geakrcccj.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gmlzkseap.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gzxaahmaz.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/glllonupf.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gaijovymq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gmrzaraou.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gllpqvvjv.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gzsazsbdl.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gjolausgi.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gellxvpwf.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/guztfzmmj.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gaknlxgou.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gdscasdrd.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/ghaqwatnx.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gpydksukz.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gtnzhnbvs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gxlbnmkec.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gpyrdpuvh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gjfwtupfc.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/galdxbdfg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gtddafjzq.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/geukzfdtm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gkndshszn.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/geoyhlvbc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gtazjqqpz.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/glpalvzww.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gkylsicib.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gfkixdscm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gggwfuepa.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gghlrjmzm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gomnuqxen.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/geyauwqgp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gzjxzivxr.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gowcdetka.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gfugeoyef.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gohviqmxy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gkusdhgfd.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gjrixlarr.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gxonkeqpt.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/grjjcbmuv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gkinwwjmj.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gersyvznq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gqwbmfgub.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gzegfjxsy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gifadqfdo.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gvvhsfqqf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gknxthtro.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gjndzjzfm.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gcprzibhw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/glgkstqqd.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gpsuvkcqe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gmvqdsrbm.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gwetmfuvl.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gprndkwjs.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gtaglbmif.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gyuffdifx.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gvwunegdw.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gddofipxy.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gzufgdegj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gkysvlaew.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gwepkdywe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/ggevkmgqo.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gusjhguww.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gzphtpccp.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gwmffkbog.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gslxpkrby.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gqswhvkpo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gxeyuakay.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/grvbkinuq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gkgpfjdyo.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gdqwoepps.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gnsndqely.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggqakfhkh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gbdzfdjqi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gglpqzbzn.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gfjakwcin.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gaatkhjxy.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/grpaejacm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gzqkqcuoq.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gczbvbnum.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gbagxxgsm.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gpombgsce.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gzdiimbvj.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gmgossxej.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/grguyaykn.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gofpovxlw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gnexgkowc.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gjljzatqn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gypcugoha.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gwiwosirw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/garzqedvb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gkefipams.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gdpegqcki.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gipeirddi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/ghgskcggo.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/geeidaswm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gsmljseiu.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/ggiulldbc.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gsgixvwuz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gfzmzrmdd.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gbscjwmbj.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gokktgkqt.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gbagtjdvm.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gbdxdtuay.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gixxpazci.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gewxsyidi.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gyhtfdqng.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gwzvtfydh.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gjuhriybb.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gltrxqoyy.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gotczqlov.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/ghurthvba.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gtczvivii.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gyyuelxzl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/ghogdzhum.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/godhjqyaz.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/grwceboik.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gnneudxea.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/ggfigjgax.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gokaipqdl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gjussvngm.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gidoycqtj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gvoxaajpk.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gdmwmgjqc.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gfmyylpmt.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/glqxcxcsp.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gqptszsxe.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gmsipzeep.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/giffyrydp.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/ggwxzllcw.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/grolqlmqv.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/ggkxiobuu.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gyrddrxrv.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gyaoexshe.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/ghftllhmm.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gfbeeenju.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gsqkeztqs.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gyswjosgk.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gjqerwbmc.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/grjezpegs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gqwsdwkyc.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/ggawgvzre.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gmofqrukp.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gjiiwvcxa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gshrkoffc.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfkwdguxh.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gkzwemnpn.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gfhdtzspq.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gwrcmbcpw.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/grlwrahks.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gzkshiwwc.sHtML


<!-- 参考信息 -->