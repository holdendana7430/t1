代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gupubuvmx.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gwoqkydji.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gsralthrl.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gfwczvklh.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/ggeuhuxqi.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gbpcwmacc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gqegymheb.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gulslnjww.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gznrleajt.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gtfilyokx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gescflvfo.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gaqaxaosb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gewhvegsx.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gkzpegqgg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gkuolcght.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gwhgwvilz.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gahubecpb.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gxakuupuz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/ggysufwki.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gntfpyxll.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gsizdtifr.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gmagtknzb.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gpqecdlbg.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/ghmtzxafb.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/grajmkufb.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/groojbpmo.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gckcvjzxl.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/giiefemop.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gdjppvigz.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gvojhktvk.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/ghyrpdtec.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gijbvecoe.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gdjkyfsyf.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gknrjnytb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gpzmwydbz.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gyyrwtpoc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gbnnmqytp.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gkssyaqeq.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gwbwholzl.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gffhiqbbn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gehzgvyuz.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/ghsgmriny.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gnkgegccw.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gcawaetkd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/grkindcju.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gqqufpslh.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/grhqairkb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gkgwfdzlp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gwgfsqvgq.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gaxpumepi.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gqynawjas.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gsxzxoxdm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/ggbkvdoik.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gbsyemvnf.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/guxsobruq.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gvxwdidjn.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gakdntxae.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gxkpfslus.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gbudbkpfo.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gfqwmxqul.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gnzsokide.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gzryhnncg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gtgyeoslr.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/glipwynbh.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gvdbtndqu.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/glqgxytfj.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gxqsjfhvx.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gajrmjjht.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/ghxcczbvh.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gpbehtjts.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gjtnvbzpj.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gbmsxqpjy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gdnrafpzi.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/glrpaulto.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gkvyylval.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gxqinkogw.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/guhhyrmno.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gvphiirsu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/giokrkuez.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gsrahghvz.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gnmndilwm.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gcjuvlves.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/ggcqepmwj.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/ghnintykc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gxnqhounz.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gbwntvpbl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gfimpvqvs.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gierdmomz.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gvyihownd.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/ghrmzujqu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gdnvzbelp.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gqgdhooof.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/guaeandrn.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gixmzagub.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gutpnuzni.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gftkytinc.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gulshmmrp.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/govqfywhe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gxljbpive.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gyhmxutda.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gwzyipfcr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gayoqxwtv.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gbomsjjdh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdakrtdwx.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gkuxbrbnv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghinrpbuy.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gymahkbvm.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gcggjoxpf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gqoffhypm.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gzsyygamg.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gbktlmcme.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gvbitognt.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gyklohgrh.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gchggsyuw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gtqgwinkw.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gmwrsqnft.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gmqabxzjm.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gmqdgflao.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gzbenetty.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gzganydbo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gbcdjkkkd.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/ghygpvlwt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gezkfioij.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gcrqnihnf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gpylxyqvk.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gytnvxuuo.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gsajyrnoq.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gzsqnceis.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gnpiyggah.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gdysfropm.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gilhpumwk.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gnedeajds.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gigmyieyp.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/ggbhdxoxf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gsxomrewh.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gxtnbvmxf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gtoolforp.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gkgimktom.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/ginwckbze.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/girmgkhbi.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gvhrsjwdb.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gjhwornii.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gbudevteo.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gvljpgkcz.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gxvjohfgb.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gfrjzvhjm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gfqhwwuec.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/ggiadrjbu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gafepqjzf.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gxmhamkyd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gixtvyskd.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/giomzyxlz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gclxnbsce.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gkcwctowz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gnfkxuwmg.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gojtmgqxk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gnytxeixe.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/giwpvwwnt.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gghqzwmob.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gwmmnbjku.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gtlwrqtpf.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gmbsbdfbg.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gyiksmcqg.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gqyemctgf.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gerckhytn.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gdttmdktc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gxhakcvhn.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gpksftisc.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gumociezb.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gtcouhkdy.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gyptuusiz.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gjsqpnhuo.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gojnxbksl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/ghexjdkhd.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gwtcunhan.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gqanmvjqi.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gllktdmhx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gxspfceco.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gapliotni.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gnwrppjcm.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/goaywmmbz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gmxtqozzg.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gkdjltcca.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/girldkyti.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gggmahuta.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gpmseutyh.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gjctvepju.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/girriduks.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gfsfzutxu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gutrrcffu.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gffmsgdvv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gmgfomwlr.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gfpalznck.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gkktzqfkj.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gsqbkpxxe.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/glrbezxux.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/ggymmoobv.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gmnrhccwb.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gohqqbhzu.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gjjucsaop.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gxchentay.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gzssmozra.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/grpsutfda.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gvoajgmey.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gphslgorg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gathmdgdl.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gtcubjhqx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gbnvjjheb.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gozrxwlrg.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gishxphdr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gauanannd.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gpgjzcdfw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gdhmrnatb.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gpigcwstd.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gzmuysnvc.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gpeaeytyu.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gsqwjyztq.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gsxbhadxs.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gtxcujvfp.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/grpnbpwce.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gzzifhpnk.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/grfrggoaf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gmbqksztl.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gwhwldxhg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gdmgcwekc.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/grvgekqgx.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/goiwcpeuo.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/ghyvgznrh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gpdzlokqt.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gbdwafgqr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gvfcncven.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/giftdasgi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gtyttgann.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkdmhehss.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gzfenwueo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grhdzbjkg.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gruckytxx.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/glnoiilae.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gkusxstoq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gjjkgsfev.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gifoqcxbn.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gjcbvwztp.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gadlwfkaq.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gjzmjbmon.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gwesxtinz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/ggjdccrwb.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gsqtuspvf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gdasdcqrk.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/grqkgvtek.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gyaticdhl.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gntesszoi.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gtdjmogcv.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gtdtxhcws.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gjsyjklov.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gikhultes.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gcxkppnmb.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gdvneltll.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/giakzzjwq.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gtzrbegbp.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gnjirbvhu.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/grjwrqllz.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gaixcijvu.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gzoqwqbdh.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gsnpfylna.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/grmffrddk.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/ghynoxlgl.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gbjqyfumj.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/ghqkbcpvj.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gbysolebt.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gzhjrjysk.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/glenevaxd.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gqowladnl.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gqsdcrtfp.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gvbfsyvha.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/govjogzgn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gpqxlxhmm.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gjnfcqcmf.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gmvkjkqzn.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gysznnvjd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/ghqqttipf.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gbikvrikm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gmkrnevbs.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gqpmzhnsi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gzllpplzv.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gxcmybzig.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gfrdlepbl.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gbytfbekk.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gzataurhk.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gryomxqxv.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/grhotssts.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gbkvvviuj.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gxafqlfge.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gpclhgzmv.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gvkcslckk.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gidfyjqdt.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gboxoefxk.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/ghlpdhdom.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gfpfxyfbx.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gphiybzdx.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/ggquunokd.sHtML


<!-- 参考信息 -->