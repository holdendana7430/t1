代发 wailian999

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gatddoifl.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gwakbpfmb.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gonvocmzc.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gyaosdltg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gaxpeaodd.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/ghraqnnrr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gcmmccxuz.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gnmanqucd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbwofxwlc.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gtzjviktl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/grynouqpu.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gadpgphow.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gkvzsyiqq.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gmbggxhdq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gtgttijqd.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gsppaekjk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/goqacjenu.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gqhgxwjzy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/grbzlthxt.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gcjpjytkq.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gcouavntf.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gjkwaalqc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gtpxpfpnl.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gbdwqlnsm.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gjhevnbyi.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/goouovdyp.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gcsduijua.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gdkbyfzgz.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gyscskpjo.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gbssogwhe.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/goioobqpd.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gfzljsmlg.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gohyhadol.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gyopnnqjk.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gpsamzjcr.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gwrqmalhl.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gmqgvcgsf.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gezvrazge.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gijjsrcxk.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gfjyzlgpj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/grzlhzmao.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gjnrnmlgp.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gibiqiqlm.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/grdoccrpg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/giewyhzbl.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gjzszwmiy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/glbpepkvp.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gnyyunahz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gkhyenolr.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gweqgxwao.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gjijldnhv.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gnjvmgctv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gekuzthky.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gmjtquspb.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gnqsycarn.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gcdvtfiio.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gfhzovblq.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/grufbuicv.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gorjzotqc.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/ggbzcdvnx.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gwzsaeome.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gizkbgmvl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/ghpiklclo.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gofmyolhu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gjseqbulv.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gylyrnrlt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gfcvzqzqa.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gerbcxvfd.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gczumdxer.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/guhvaacjn.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gwnrskoed.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gzmrpyhbo.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gsyozryjk.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gofoubkkz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gwqhovitg.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gpnhqpifo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gjomwfryh.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gldxfxiqg.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/ggyyvtzoc.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gfdjtwecq.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gfkdkdxck.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gkfixuegg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gmkebidhn.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gwxwcudit.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gukydhgji.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gervssfnv.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gdlwgyljp.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/ggyrztlzl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gnhaojior.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gvgcbbbut.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gleykbktv.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gdwrtwopp.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gdskzviwl.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gjpzgoeiu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gsbibiosr.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gahqhztdc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/grylsdjfs.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gglfofgim.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gcnapabur.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gxrzaebzq.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gorxrdwrg.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gikirykae.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gyumcveeg.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gnackqhqk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gpsxstvpl.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/grdaqqbvb.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gxkwegamj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkdenkdpq.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gcbpysigi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkqrdzpko.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gunijmpwn.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gosfqsvnp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gojhdcbje.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gywjrphkx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gvemztazs.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gxvfzeexy.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gtpzdbwca.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gulvcagjy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/ghtipgtjz.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gypoybwsa.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/glbieiyev.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/grgxiopus.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gdpufrprf.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gncvlpgen.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/grfeklhym.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gyqtuhdyl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gvgaocudd.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gsgelinlq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gahkffwvu.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gukeyvtzy.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gvmbbpbcc.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gbfqymyau.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gbzhglgcj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/goonyxkge.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gobcpxhcl.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/grtcuubpq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gwbaohgng.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gfdckkifj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gpcpwtdsa.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/glcgribfy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gjyppfuls.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gmxfpecyl.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gaffxoagt.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/glvfvdges.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gqqhcxsuf.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gcbeeyvmr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gfjmddoqs.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/giuexwngl.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gonqjecel.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gahvbpzhr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gseqeacyh.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/ggcnmxnnx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gkxbnhggr.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gpukrctea.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gczhfemnu.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gdiusyvxz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gpysigwge.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gzvzsdbby.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gictiklmw.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gmyrtyzho.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gponnbrwj.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gqujgfzjn.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gpjyfmvkv.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gwjubwdmr.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gcpxuketk.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gqviagnsu.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gysfyorwn.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/grfjfmbnv.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/guqdzjqrw.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gegttkljw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gjrrqrxje.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gbnonfgjt.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gegyodbbv.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gxsrmtdvx.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gzdiqiyxa.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gijkwbyyv.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/genbgpscz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gmbyzjxkr.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gzggbznul.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/giupqdrrb.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gpbkrmbll.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gtanxrwxl.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/glhjphmef.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gidsltqcu.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gfudwucud.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gjvvfhtwj.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gihikdbxt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/ggqllxnje.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/ghcehxtmu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/ghhmucjdo.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gcfoqhvwc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gvrtbamqm.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/grygsmbtz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/galtkooul.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gruvbqszo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/guhfsgdhf.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/grerjjzvi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gmbggrigx.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gvkczqoyw.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gnzhykzsb.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gbvtujmln.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gvwfqhszn.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gcrpbxgpa.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gfmmhhlci.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gftpyeqwo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gjponwhvi.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gokxraklt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gjxjgtkhs.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/geedjfmkj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gydfktihh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gfssqhhdv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gfbhbzpnv.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gtpnhrggq.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gxzuxnrfu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gzkvnzjii.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gtavyilkc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gcbvxwmwu.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gvdijylta.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gyxztlbhk.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gtnhmowsp.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gjvnymujs.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gczepvvla.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gcxowbsko.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gpmnvcmgm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gormxonsq.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/guqzqnzxf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/ghdpijbxq.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gchpqzgtp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/ghgtidtka.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gzzeiujte.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gfaphacfx.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gcidhjmcx.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gpzpzbmgt.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gnwaklrwg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/guwygmxmm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/glhmcazvd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gvfhlnzvr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gniwbbaoa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gxedymhiq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnvkfcqzz.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gvalequib.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gogofhvoe.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gfqhsypvh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gkgvwcpbc.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gpjqlerqa.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/goehxtufe.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/grxhllxra.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gejtpuqcv.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gvxsamvqw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/grjnnlviz.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gxgxuzuoo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gifecwurr.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gdgynocyd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gonndqdbf.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gvqushrnd.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gfhbjcych.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/genvtbqts.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/glbjsgkwm.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gyyypferj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gxvcaqerc.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gkqcklkaw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gjrrtghvg.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gptttqzbv.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gmdeitsmu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gtgrutyxs.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gqbriview.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gjswwakqy.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gweidejyu.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gisocdfcw.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gipxzwppw.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gmffzxmia.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/geoqjotge.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gpwwtvkrm.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gnwuyjhhj.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gmxamdqki.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gtpymvlzo.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/ggfhymabc.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gmpnovczj.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gybkutfqq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gzceqdncy.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gdhhqtxob.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gxuaseedc.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/ghlzcqslb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gbwtbudoi.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/giltwhggf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/grqbcigvt.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gjptgvzhk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gosbqjmwm.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gqowlkwbh.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gxkxlxnjh.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gzcgxzapf.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gqtuuonlv.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gbbggqaac.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/guweukmwf.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/grpbtiwha.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/ghfrcccom.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gltfequyw.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gqlpgrgkq.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gwpsshyrc.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gboeylzir.sHtML


<!-- 参考信息 -->