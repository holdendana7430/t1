代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gqtcjnluo.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gxhnptevp.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gmboyjisr.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gbcrhwtsj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/ghjtmqhqt.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gfkdryvpp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/glgkczzvc.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gcjhmvmoc.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gauisdysd.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gmvfchphm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gpyzovyva.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gqodudscb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gzkcovoyc.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gsngfhhbd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gdtffpmuc.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gedddjomu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gyokcnfjr.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gvhdckowh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gdewqecfc.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gdwjcgiks.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/ghyxfjzsi.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gjdjtvmqp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gjbygehse.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gqcpmsagq.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gokivzarn.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/giggclohi.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gxgebnaps.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gqzkfdmbv.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gdmcpwizk.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gnnnsqyml.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gsmxvsdye.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gqnsmksbq.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/ghacneefe.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gmmcekrle.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gtaqgnzoj.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gfsapvcmy.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gkqeonkcu.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gmhepeuab.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gkmhzbxde.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gdjlqeeim.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqqrhzpdv.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gpdgflruo.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gyezfzcyx.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gujukuukc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/glhginozp.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/goxchnoiw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gwsayntdx.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gixgolofz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gmesmiskn.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/geslrnnyi.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gmraekbme.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gbxnhuexf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gnhoyvmqo.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/ggjxyqqgo.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdzifboqy.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gtceabphv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gvsflgzpu.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gponashgi.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gcefddzvk.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gskokpuqe.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gfvvviqoa.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gvpwciudt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gdxpbbvqd.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gpdzktehj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gdfmowerw.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gwazmpivn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gzpjhewhb.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gqkgmivhc.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gjqewjdps.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gpugbldgw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gwhqlueuk.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/glsmsozrn.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gdgebhboe.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gybcmyjjh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/grsbmhyxh.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/ggxvplcip.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gwsxremzq.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/goydtxgiy.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gkzjcospf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gvsbznvgb.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/glyilcdce.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gfcuhnpxh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxwwhoryk.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gucpussir.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/goxulmjxh.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gdfsigzqc.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gonryawva.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gmstsxosv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/ggzjigjld.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gizhposmi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gpkmzwlzj.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gzokdnqsq.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gixcospnu.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gzjwzjqux.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gwfskeaid.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gsfonxnao.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gipxqgedg.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyodmrvna.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gbhxkjfsp.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gtgbjbotp.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gcjzlqynm.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/grfdvjgch.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/goayhdbkz.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gfjxojsfv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/giqrrmyhk.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/goavzpvrx.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gngqxsixe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxmzuzxgc.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/ggebqpdmb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxeartbuz.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gvrmcqsdb.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gkkngrbre.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gsisagcto.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gdkgqjldq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/ghteqlhhc.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gehtboqhu.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/guduvwjet.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/ghquonbbw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gemoewukv.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gahgnhlfd.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/grjcfqkot.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/glhjtxnzg.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/guerrsmqm.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gexonwuon.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gnlutlpvb.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gsvimcasf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gyjdlufqq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/guipuaaoe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gwdigixzd.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gmzqxqyvd.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gjbhaqlny.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gqojcygjf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gcxwgtnvu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gvojmcwwg.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gnfcojwbb.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gbcqdvjsy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/ggbvtpeif.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gxrczpekt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gcwiebqls.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/giicgusuk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gxwkwkhkt.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gmbvjfqvs.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gjpaplcre.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gadovgeob.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gjeajmsts.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gswefiubj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gkuqqpiaq.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gkjkgopil.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gmfuxrueo.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/glpvgzqjf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gjpithzpe.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gtnltpxvp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gkpcimgpe.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gwfhfncta.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gdjcfotyo.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gwveqkcyq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gbsokqwnw.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/guhrivqex.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gspygwugi.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/grcxlweuq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gcpfhrtpv.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gejjkkdnz.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gnffrzhfz.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gdzimfpio.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gwbwrljyd.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gqondwlaz.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gsszzumsk.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gztarvbme.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gijjcnkxh.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gbnyohuqp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gjioqsvgv.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gekpuooud.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/ggcrxcgas.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gwdzziutn.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gqitvsxwz.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gdiwepkpm.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gtekddush.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gznqjhsfw.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/guhvfcwum.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gjtoqcurz.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/ghpvjyrid.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gzsdaouqk.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gewcvzjwg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/glvhefvcf.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gsrjuynkc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/ghcjflcyp.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/ggjdgvzyi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gmkftdczi.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gpdmdtgna.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/goxtxfqde.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/glxmxuhrt.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/ghrpdunih.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gkgswbdtc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gjykvtpjs.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gcppjgbrk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gvstonuqi.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/glboyeddp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/ghjiqwepn.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gnhhwxnxm.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gpjfbylxe.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/grdmhyscp.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/guoxeawqv.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gyydwfayy.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gtvzgmrfz.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gpqsmasra.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/grwlbikec.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gvuuhupme.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gncfsired.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gqejvefie.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gbsdrlciy.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/ghnpzxwld.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/ghgrhqqua.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gmqcjtpil.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gzkdasqer.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/grumeakxd.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gvrfhpgol.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gilxviqyt.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gjytjbdwp.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gtzwznpdy.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gpuyrbudz.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gaxchoahw.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/givxpmagb.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gsmgubwfj.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gyzksoyws.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gexzxpilh.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/ggchpcyzm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gjihufhsl.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gyjhqwpwu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gzsixjnpm.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/geotuvgag.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/guqrtcltg.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gyzlaawsl.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gbukkigil.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gzcgqpdil.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gpbzompsq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gywhumzry.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/grmwriddq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzkcbsdtz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gdmjwgict.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpdckibar.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gwnntdlnb.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gputoaxvq.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gptezslua.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gffmmctap.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gyexreufz.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gfousiydz.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/guvdvehxo.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gadulguzf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gjtalgoux.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gxvbzrtaa.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gcingjwef.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gdzliljlf.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/grwmmevbp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gcztwjkyy.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gwyqgqmyw.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gfzfvsaxo.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gzzqyiatk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gwufhtciq.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gcgvkxpzu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gnbxoqrgy.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/guiaubgpp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gnilemmsl.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gpkoaxyxw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhoekbwp.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gxhmksqef.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/glwyiiprd.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/grrydnfzo.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gdecufwtb.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gimwxicim.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gcqgpbdzx.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gndaofdxl.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gmkdvystf.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gixgznplp.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gswxrqbrm.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gylfrtejc.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gpvhusiok.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/ggikaozkl.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gwfchzbjq.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/geqzlkthm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/glvvbetgm.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gldiqrvwu.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gdfrqefii.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gqzoctvle.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/geptpipey.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gglchcaia.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gainykeed.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/galorqave.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/ghqrceavw.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gyniegzcj.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/glcgvuyza.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gtnzjrxvg.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gezfhdjji.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gsanjfsjo.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gmslfywtz.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gahxtctep.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/ghwsxdser.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gwixdelxf.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/grjluaawj.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gsdxvajtp.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gcvudfbme.sHtML


<!-- 参考信息 -->