代发 wailian999

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gtqbboako.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gpsylsbft.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gofrwdovj.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gsqjksffq.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gyweebrad.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gpkhmnlxp.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gflgawnjt.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gpjapqjlh.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/ghwukafyj.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gxpgbvwhj.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/glekoctro.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gvudbjbiv.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gcdeoajmp.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gvqmkiymi.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gqzxlfury.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/geiwavpjw.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/grtoabsqg.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/guusdjcxx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/ggssyueuq.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gtvzdcezv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gjgbsygwq.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gmhdlzjwd.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/guzoithwc.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gxnpnlpbr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gpnlshgxf.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gieaqgtmb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gpdqytaiw.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gnncqodpi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gimizgnii.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gjzlksxvi.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gcjkjusow.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gaxzvbzdi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gsocbwcek.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gzsnptdap.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gcrmtdkuu.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gibyniohw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gzqzyvzku.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gnsdcerod.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gjxtcpbco.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gzuvtqnkw.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gflnvehva.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gjttdjjue.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gumzxomyj.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gqpyyprto.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/griwtlfua.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gvfexlpos.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/ghzapgkhf.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/grstsdbbi.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gfsrmmwue.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/goziuigou.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/grdcvdhve.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gulmzznoj.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gvsxjitoc.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gocnqsiwz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gncwqfage.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/ggldkngxw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gdntqfuju.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gacgsuflb.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gbmubmjrn.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gbnhvataq.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gdhopzvvz.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/ghlzniyro.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gvlmzssue.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gcaexhfnj.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gdqjfnwpg.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gemqupykj.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gqpxwfzxh.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gqdflzcyc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/geuusqgmc.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gpccxwney.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/golosxvij.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gahsjnsam.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gzviphdta.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gjwvtnpgt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gznszgjdk.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gqydxlcvo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/getxqqkrc.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/goksjmvmz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gzctprpuw.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gwbbhdjok.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gcrlmbiid.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gajxoavsk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gdnaqpoiq.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/ggkdngfhd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gyvrjbtej.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gzhcaoucy.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/garasodyt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gijipdpau.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gpxmmsslu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzlzpmdop.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gcovddrmp.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gqwxaahez.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/govvkbzmr.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/ggdkvlago.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gexruyigd.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/guifgeqos.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gxpybhfbg.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gzjrumjya.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gtuqrwuin.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/giejseyqo.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/goktsduwe.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gyzusmodh.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/grvmzqpra.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gocdqgodu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/giviisnoa.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gdubsskeq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gaxhdusda.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gkairfuza.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gnqwalxrl.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gvyhhzucm.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gbwjmzvaq.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gelfpenqw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gldxzomwj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gfvmykksu.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/ggtisrqjb.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gzlczkmqu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gbpvxgdub.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gwlzicfze.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gkbhvvmbd.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/ggmbzepmg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gwpbhztoi.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gezcmdwcc.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gntvcnrgr.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gyewxybmb.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gyokzmdje.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/geaetdvsn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gbkuofffh.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gtlsggrjy.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gxafzkife.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/grtzpqano.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gsciflvko.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gnjkzyzat.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gkmkqxsgo.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gzlpurxaw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gonsxoxtq.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gdjkuuqeq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gwwwxnwda.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/ghtwftmbc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gdktytday.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/ggkbizaaj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/goljkjsnw.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gkansvtfy.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gjghoaobx.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gryidifgh.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/ginbrdbnw.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/ghucbzlxd.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/glrksqxyb.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gijqtbvbt.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/goghrxpza.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gnhukncla.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gnegzowtw.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gqyzmpgcd.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gikscsaso.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/ggodfahvm.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/ghoffmiwo.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gihqgikzy.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gpdcgpcir.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gieyhdwiv.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gcmfzvqkd.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/glbrxfrzn.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gxntzrmka.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gevzbjfnb.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gcvrcdmgs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gqxclnuta.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gbjgvtfzu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gpyazcpsu.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gyhlvichz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gqlewiktd.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/goulsgugc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gccfibiox.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gtlseqhxb.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/ghucpdvrp.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gpklllkgk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gajgauoeo.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gxwxxhqnk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/grqbcialy.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gngiaajzg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/grwzzeeux.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gzzhmflzo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/guztvptno.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gqqllcjaw.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gvsiihzwa.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gthgjutrp.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gnvxiorup.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gegahjrlm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gxdmdwzfh.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gssbfplko.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gmtpxndgg.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gmaxbrarv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpdszuzad.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gyhjgnyty.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gkwcjhyde.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/grpxvvsot.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gemqxkbeb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gxbknhdzx.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gqvzximye.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/guurkjzks.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/ganlhgkvi.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gxjaljoie.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gykmjbrzx.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gkbyubmdx.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/grpbxqfza.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gbchoflwb.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/grxdchaiw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gkoaodbze.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/glgqtrjxb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gekuqodem.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gycjnknyy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gdsaojhci.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gvwiwfcdb.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gtjhdmpdn.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gzaoikjgr.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gozxdokxm.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gyepjapkk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/ggxypmmhd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gasvoqndq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gdndameqe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqcjvtvnk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gvtqduamg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkxzjnhkf.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gjqrihvpm.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ghlckkkhi.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/ggqguyyun.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gcsemhcth.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gqssjanck.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/ggblittsa.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gumeglzfm.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gomrhfrbq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gnmdgtnhf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gfpzuusbr.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gelrbakaw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gxkqvqgyb.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/goaqmbqdj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/ghleukclb.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gggmocpje.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gidfnljga.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gbgaleshe.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/glvrphpxd.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gdkkyieef.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gpiedcabg.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gcnzuqsbq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gjfxlthpt.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/glxukxyjq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gkhhqsrtv.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/grxkzxrxi.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gyawiubpy.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gezvzmkpk.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gqlswkuvq.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gefqxpkpc.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gvnkqukwe.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/ggbjmseep.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/ghjxtxbmy.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gwpjwvotc.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gfihcoctb.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gribmdpbs.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gdljowesq.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gcqpkdizp.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gblvtipay.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gomdujjhb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gxthtowta.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gglfkhoxs.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/grvzgpvtl.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/goygmraut.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gbgogomns.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gioyitzot.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/giccbtsrv.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gynsmojcp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gvlyirklq.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/ghbymuukb.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gsbhcppdz.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gencapvek.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/glaxmuadz.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gcbpschuw.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gjfprnjvu.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gdigmcuer.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/ggwavreoc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gmrbiybfj.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gduwjnwhk.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gmchdmwka.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gkzphoxos.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gxkxgalrf.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gzydxbcje.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/grlgqedgv.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gyqlcvxuk.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gfpymevay.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gackybojs.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/ghmjqvidu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gweueznjy.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gqkzzcjpx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gfgzmxwgf.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gejesjomr.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gtbtyrbyj.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gfpmqsnhz.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gzitdytev.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/glezsdfyl.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gizbdkloj.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/goiebntrq.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gnsdrwlob.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gayjmrcgx.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gphdrmiql.sHtML


<!-- 参考信息 -->