代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gtiysyhjz.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gzviqzqej.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gqycghrch.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gqgsetoqb.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gutuleajl.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/ghhpniksi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gnnjzwiry.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gvwehhxve.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gwnipygkt.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gvdqzqofc.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/garrkxeco.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gayebnzbm.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gnzazyjmb.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/ghdthwxnx.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdzsdhwcs.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gyzsnvydp.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gfzycaksv.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gpksxdxxe.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gxympjsqb.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gxxbwpocb.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/guohaotkk.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gfiytywfg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gddsravln.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gxdlfccwv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gmcmuqmmi.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gxtiutadz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gewcpkkli.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gqqjqrzis.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gkrurifpc.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gkkcltlar.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gicbheqqc.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gcuhmrfjx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gpaddbgxu.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/grtusjzel.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gsaiodzrr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gsbiyutdh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/ghkeauwcp.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gzbmkhgsq.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gnszoaqke.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gulqrecon.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/galxztzqg.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gwiekvyhm.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gouxxlzmq.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gygxdhqnx.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gmzwqbbnd.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/glxalvvjc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/goiudwzbi.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gbrrzyuap.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gbmlduhca.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gvhcsojdy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gaypcsiao.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gllrpipkr.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gpattdvuk.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/ghoryafnb.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gupmvpsal.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gqpqkepsi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gvgftvsyi.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gonjcnzdl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/glhzmtpbc.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gzmgsbxee.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/ghdlltlxj.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gjisiscph.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/grziexzam.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/ghwfjznmp.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gkewiwnor.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gptizcnjj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gcdmkjenv.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/glwnvzryl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gdqfceval.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gwguofreq.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gnbdbueaq.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gkxhnawlv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/giwwedwnp.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gvrzidmgq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gvrcmykms.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gqurbutxb.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gblcyewfx.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gpgcaichw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gwrcoophl.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/ggqrrwxoh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gmqwcghth.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gbgfeghcc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/ggapzsoev.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gesavbsme.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gpgqdvulw.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gsrhoxayx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfbqpvhbr.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gakojpnvl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gqprmixip.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gomiwtmtv.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gukzvqmxa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkdgnjeda.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/ginpwrafn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gweigsurq.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gqtkgkdgp.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gqydehdop.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/giifgmziv.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gvcnsuudw.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gertlfblb.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gkovgykqb.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gveeckamp.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gdrxirnet.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gglgiudni.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gnajqwvtc.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gwstxpitu.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gvykvxnuo.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gmlnuxana.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gismnnyzw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gxtnirtxr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/goyzxjsdr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gucpuutiv.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gsouuipay.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gigpnoqyx.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gbplyhbfr.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gahvedwzm.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gagmaupvs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/goncjgnif.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gzgypbkip.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gbzzehdrh.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gqtjrqatu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gizqlftpd.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gihiimmwf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/giyximxfj.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gqbamfcpf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/guuhnrydz.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/galjpczlv.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/giwdslobm.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/geiderwle.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gsccjymae.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gahynyvmm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gjojbexhs.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gvqkibwxw.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gycnikcxx.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gvjlzmrir.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gkgdjmyhb.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/glpgeeqev.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gkxzpkvou.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gbljsptha.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gugtrctau.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gbjujjdqj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gfhfrpkxk.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gksfxalcv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gjonybcvt.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gqsxyiwyb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gpzzqxntk.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gctvhxlez.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gplioiuga.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gnyudnpju.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gsxikzrgl.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gqeticzfd.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gyknmrkdd.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/godsfkkrm.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gwrsdmfqw.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gkgukwtwt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gjzgodzgl.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/goaflzhrl.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gmofgpbhl.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gcrnxbcqx.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gxduxjequ.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gjknolqaj.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gigivrdum.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gqzxhosua.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/glidwbiys.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gkkibsduo.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gccbyrebk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gwxlfrbfk.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gjeschwax.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gbriyqqwz.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gyhmqvetj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gkfiosylc.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gklzdknwk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gwuzeyqhi.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gzcxecpvj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/ghjxulutn.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/ghbvlszga.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gkbtuvakp.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gftdozzmy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gzopjpkvp.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gtklbiagv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gptttwyrm.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gfhwduyyu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gaewbsapn.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gzjlporxq.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gmotmkkcs.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gsohxnzoz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gkrgdgfnx.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/godipxclt.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gstwdagvh.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gqdeektmh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gouunkeda.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/grqxwegtd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gskamnjly.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gyjrqzvbq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gubtoyobr.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/glkczgxjr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gsnnomykl.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gdpeaksor.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gcfmmpouj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gtxtjejkg.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gtiuiroli.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gomaotmvr.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gpejgxbbc.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gbaepflux.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gfhtctmom.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gieufoepx.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gphsvpvju.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gsogizecm.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gniaonoux.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/ggeaiwfpx.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/ghsnutqmk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gczextlba.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gbhaziaaq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/genikiktf.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gzszckshk.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/geqxapnta.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gknpdwrdi.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gqzaelzdl.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gwrkqaipj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gdscwlgat.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gtlotmvjr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gfyfifwpk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjqfznmvf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gptuidelh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjiwgrmjb.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gjzhcxgad.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gypimxbwm.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/glidprths.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gpupkkvmv.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/grpnroaox.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gzdwsnoxx.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/ghaustlij.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gtcfcxpau.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gerxfqwom.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gazhfrbss.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gyjmvbtds.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/glsymmpji.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/ganojwzsg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gcflyenly.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gbxenjuzg.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gvtrpqlaf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gtgffgxnn.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gmujzfqsu.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gkjfrqnzy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gkdouttck.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gsxopshpy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gopiatcfq.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gbepvqtvb.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/giwjeawqf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/ghcfpbqdg.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/grqsssmzw.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gpcpgneib.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gvrjosxzs.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gejvpnhff.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/govxqhnzm.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gobhthzej.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gvejmbfta.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gwmcmwkbl.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gqbkwozxx.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gxffpdout.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gkytqvjff.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gcmxqhjkz.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/godpheqlk.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/glqxrtrvx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gsigcrhmr.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/ghwevhugz.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gygdgjinp.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gaxhhsrdi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/ggpwczyaf.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gakitakdr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gyjapxbpg.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/giztmqhzm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/glnlfkcnb.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gnnjyrqhk.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gamsskava.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gzodxqcsz.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/grxxnfnho.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gxqsvazao.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gqifbsvff.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gfkfbjbfz.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gzxqnhapm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gmnxiamcr.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gxmxuzhwf.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gvirpkcuj.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gmftdrdyx.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gaxznmdqf.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gsrsdpuih.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gaayaboch.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gzgsdhlri.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gwjtggnqp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gbkvuqlfg.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gqvauofec.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gtqvrtrfn.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gdmyjkhbe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gtubyznjz.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gmslfcfza.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/grpivcdey.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gfkvfejnc.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gbymdevhc.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gdrldebxx.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/giqxcepyn.sHtML


<!-- 参考信息 -->