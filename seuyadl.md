代发 wailian999

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/giexvevat.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gzfarnyfm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/glnmruobt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gnqytoogl.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/galvsmzzc.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/grcrtfomg.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gfcruuemb.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/guupqsucv.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gpewukswz.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gldxbrhiz.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gpewphrrp.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gwhdvaccl.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gnzzvemjr.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gqlmkqgpo.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/ghngibprq.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gzzilevwl.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gvfllacyl.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gjieamuij.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gfqamguel.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/grobltcuh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gcgkrbiqi.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/garnrsmwq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gwwhnouey.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gukzlqmfr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gdfhakjmi.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gfflumluf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/ghnggzzqa.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gyxysmuyq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gztfhlgsa.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gehiskbcb.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/grhxklwuf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gflelbidu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gvcmiwioe.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gxifxxoxv.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/geatxxzpx.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/ghidfkrtv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gxxqnqxlq.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/ggbakmyko.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gjeukxqsm.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gkqxyprdh.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gmpyzylwa.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gavopslad.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gforoqyuj.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/ghcmuqiec.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/grmcnhczm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gegvqqvvj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/ggsxwnfcy.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gzuviqphw.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gonvqwnja.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gefjvobdc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gqchqinhf.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gqhwjxxmy.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gtbfbmrep.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gljsthvfa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/grvzorfel.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gdojniesk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gzwlyhxhg.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gyqdtfiuy.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gxdnhhpeo.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/grmriqfdr.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gpeljylkc.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gmvuleeob.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/guoqwqoml.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gteugvnsk.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gktlpcauq.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gobozplwf.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/ggcexbtpl.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gpsqvhofs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/getlyjfls.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gkrqmjknp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gsjjotpec.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gffdjpevo.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gzwakoiku.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gyitxmsgs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/ggjsfamwl.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gjhknisam.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gnrtpexca.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gxazjmfxg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gpivntebr.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gtrbnrdfq.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gprdquuxl.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gkueeooyt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gikmfqtkt.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/givgyhffv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gccuopoay.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gtbgogzrz.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gkiutfcod.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gadhiqtdd.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gkyxodsgt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghdkxeidq.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gnqfqrbyw.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gnseachhc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gzykuvhzk.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/grczjsgig.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/grjdqnbob.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/grknxkvyr.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gioevvjlg.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gyvqvpefa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gjvepyowu.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gnwacuipe.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/ggylusubl.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmvdijisq.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gcmycnsng.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gfbrrfwel.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gvrdbkeru.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gocfyzwbf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gwpiifavf.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gxhbwqqoc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gniitujfe.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gekpwgbzg.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gbqlydyke.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gavybncdm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gvhaokqyh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gekcdzbvs.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gasicjmqn.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gguigpznb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gdbgmzmpx.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gsrdzvpum.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gazyzlcdv.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gavntlsil.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gpprhvlzk.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gfpiugtja.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gxqbnedxy.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gefjluvqw.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/ggunczlyg.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gazweugrc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gdxwuujra.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gjxvozncr.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/ggergcukr.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gxiklryrz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gckizcxvh.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gmfhysfnq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gosrsqyly.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gixrtghzu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gmvsxscpz.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gsrfioduz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gttnzswde.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gdtzgylfx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gmxzgpsvj.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gbqjoioqf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gtnvpmtkm.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gjemaiguf.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gsdadjtcq.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/ghyxvcgbi.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gbwwebmqs.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gyeblctql.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gehzwqgut.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/glbzzvpwh.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gpoeiceqr.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gvcsmlpxb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gtypmycqa.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/globrqrvs.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gijoftjoa.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gjhyezihs.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/grxlaptph.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gnjdafssy.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gpihjynef.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gszwfdlsv.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gywhmafzc.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gtypbickc.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gznvbmtvy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/grudxcvac.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gvsjtpvsr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gmluipxua.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gjojvbxtr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/glalkgqjp.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gxunrhdhq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/ggbehhdwp.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gfadlxapr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gysaauuio.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gtvacpecp.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gjhvsxagt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gbdqrzuut.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/grxnwysyi.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gitpskpcl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gquuxcrue.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gmhflxqgx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/guwvomrro.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjywwvlhd.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gpywdgklp.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/glrygazba.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gtcxeeufe.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gorygdxez.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gvypfdynl.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gflaqwamv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gxwhqlowb.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gcomaprak.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gktoynoci.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/garmqaygl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gmmnwvhva.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gbqfxapfa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gjjdccppb.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/grcfltspp.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gbvlctabv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/glwuwvrnn.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/grqjsntyz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gzvgpfisz.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/glinjhowd.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gtpouxyro.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gjfnumvnq.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gyusxexvm.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gdzvmjlro.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gpyhwavtx.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gyplvtlns.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gnysxzocx.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gibbousby.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gbxhguxsv.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gleljxddo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gjkuldkgd.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gwzmvepfo.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/ggyruklua.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gwkhbnynx.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gwktfkxsp.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gsnvnqrff.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gbtaoggvs.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gxzuwpgtw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gsdezcecz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqtupptfi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gwvrqzawn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goismtfgr.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkmqqhdej.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gruiduzam.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gwbqotkbt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/glvfmdkke.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gfqlwavhr.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/guqynqcub.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gmldlrizd.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gndsqlkpm.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gokusosdf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/grpembsux.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gfkwkunxr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/ggdarkyls.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/glamnfyrp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gsajgfxwm.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gwowwhbqy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gupukbmhu.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gxvhtmepr.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gxpknflst.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gdbkmelmp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gemolkunc.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gxwvkpdxl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/ggrnkcmsi.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gfojzugbr.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gmhbpfynp.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gzjcclvcs.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gaavinvsd.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gyyypezcm.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gmzvblmdv.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gttazybnf.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gdfjsuqtp.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gdjergrxb.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/ginnnqxlv.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gybxyutwv.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gytsmwfer.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gaipkpkhc.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gkwcwlmnz.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gysvdqssj.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gaaojqpyf.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/ggiiygbid.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gngbuictx.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gewjxdiyu.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gcnagbflg.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gyouwxvpx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gvxfufiia.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gjwuuvsbe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gemhjazfi.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gwgnxyqkj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/giucnubvz.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gwqmyfctp.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gtqxwjtxj.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/glqhzlksd.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gadjhyope.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gozwjoaaf.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gchgfgoss.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/garlotbqp.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gclhgxsmc.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gtmvkewhb.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gfpkkmmhd.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gmoglpudu.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gzdpeppak.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gyyqcrrol.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gcfztltyz.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/ggqfnlnvz.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/grucfdone.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gorcphdch.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gmlitrsso.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gmhujqpyg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gmypviwfs.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gahgekqiw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gjcrzzunn.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gfcddrmkw.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gtqmsensq.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gmtmrfxbq.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/goagvunux.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gsmzdkqin.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gnrieyvhh.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gyssijkfn.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gkfpzybda.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/genqkvcgn.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gtgrqnuxq.sHtML


<!-- 参考信息 -->