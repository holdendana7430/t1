代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grrukjdfw.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhesvptg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdpnzkojc.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gxjdujzhh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gsdfaauna.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfgxieen.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhzwlnjs.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdhewbxb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gupmnhwcu.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzijafmv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpvjnxrq.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/guczmvaqe.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/glohagkmh.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gzlzyvrlg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxidfxepn.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gnadyvtpy.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/grnrttsnj.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gqdleayfx.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoexthwj.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gpyvftyzs.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gfuaphidt.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gnhtqglix.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glpcqbtbb.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtvxuhgzx.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjuiubya.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcxjktbj.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzuglhuj.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohwahcmj.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknscekxd.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvroykirj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gsvbkfmyq.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gqahjckyl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmkuckan.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaolldgm.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjwklvnyx.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gnysqqhqe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgetvmvf.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxyndsar.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grpzzrsfh.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/geclrsgkn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvitwuqq.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhnvcgrn.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjacmpbq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gpkaeaihi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gdugpgvyp.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbatqxmuv.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmynsfyy.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gficbzzmi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/ghkkgxrvc.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/govgqsxsa.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwczsuisn.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggteovfd.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gbbvanvkt.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gklipoelp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gjuagytoj.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmedyzqq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnfzegmk.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwdgiqox.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfsspcuv.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsomjkmi.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmdhltzy.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbosurogv.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gpsoyzgqv.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoafyjjm.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gbgslqnep.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gldzjjgun.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprdqbskw.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gtfqutytm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxuhfwoq.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhtgcnfv.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhbphwnm.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gmmbnbnpi.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gexbwdnoy.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyygqizd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdilufojb.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gglswvjxd.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gejaimgmi.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gspzlmdug.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gushnyusv.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnutycha.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipkxface.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhpvvxxu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfttuqrut.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/grbloydbs.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/ginnuhyxx.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gilxadhdk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/guonpbvuq.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkuqcknum.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gsxbgskib.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gayepitsk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhwdjoqi.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gnupusmuk.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gqglohwrb.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/grjsevtwt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkedzdur.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gsmjaoivq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gilskslpn.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gzzpeeagp.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqnsafcs.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxsyfaqn.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gjllmekjq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzevauagq.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdxilwfr.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gicxsnjku.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfnsuxtto.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gqxuovgyo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdobyyca.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkoparke.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/ghwdlmemn.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gfmlksmte.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnihsupsz.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/goswjjczq.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/grckwrgly.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtvxetib.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gacxhfwfz.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxnozzlv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaqqaqef.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gyjpkqolu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gylzxgiaj.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gbkvyahjf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcmzawzn.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gjsadvxip.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhevfwct.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grdmxqmqd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzggrclh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzcksbqj.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gkkaukujj.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gddwlywbt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruucolkw.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhvqpxwl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/geanyffja.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gbafjugzu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/giyqqeyzz.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsuibhcx.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gkodnvmmq.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/guypoolfn.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpdsbbrp.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/guhklvpsi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqokzddo.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gsombxqlw.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrvvmsaq.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtnbshvh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyotbtibk.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gdnptrqec.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcidagyip.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxmwkzpv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/grjbteemh.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxhwngln.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/giqdiqfia.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/glclvpshg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweuqmdxa.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gyilztdno.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmishjvk.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobqndwgi.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganjklivb.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjceyowe.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/ggeeacwsr.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/giatlapmh.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyehueiq.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/guwsbhgtv.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmszrysvq.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/geadmbhxg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhoupvnq.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjslbyczd.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzsnyanp.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gcavrlljz.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqlfxeig.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ghhcqkdcf.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gnbreudtw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbbwqvzjn.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/giwhjxfdi.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gwfqdfiyn.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmmhphgd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbwskjke.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gloqpvxtw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/goanwnwnn.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbvfchgz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gtqzyxnnj.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gucmtekju.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcnomywf.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/grzydhdry.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gbkhdbnjr.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gruophwcr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfajowdj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/guhuhhnyz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsnnexmr.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmooyrkld.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzjsdpkb.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gobypwvtw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gsvlclxal.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gksqoyhyb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcizvvrhy.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhopqfis.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwytoeonq.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeufpcfz.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyxzfcljo.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gqrqlvxfk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgqbdrla.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gchnxzoxd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gedtjyada.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfefapqi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyngmqyzr.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfrsdzgk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspkvewdp.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gfitrrxgy.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvunpgwf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcfjkwol.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gdagpptff.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxztjtqlk.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrxdfguz.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmmjpdxs.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gntuoduyt.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gczwhhqbo.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/grwbkrmib.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gpmrxppqu.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqgapsuw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnniuadkf.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gpblobvpv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gclwcsava.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gywburbiu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkhgqsvqt.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gilvygwiu.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gubyuejms.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gydxtxuqe.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/girrlmxtd.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gczcalgsi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtydicqaj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnskviir.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhbqiwdg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gytywoybc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gkjltdiev.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/goijbjalh.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqllrmfty.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gfynfwqla.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkmsfxqkz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gqwpybmco.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgiqcesy.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gyhnfuhdo.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gvinypccf.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gnhmrjvwo.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdkxvvcf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfqjbrhc.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyharjue.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwxzohgn.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnflnczm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqorstcs.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giznlvrrx.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/glrgmuupc.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gexcltiug.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpmhavia.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gblvnkvvr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxzlplio.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/glmgjokok.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjenenua.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gjcguyrwu.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmdzttiw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuvqotuq.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gkdmrqncp.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gihfkyvis.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/ghuuqjvya.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gvhhwjuui.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gsqimvcsp.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gostoffrx.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsckepiwh.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gewtvzggh.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpltpswut.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/getkoieug.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/groimalyd.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzcpxasy.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlgtghjg.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdeoyxlb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gldqprmik.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjqhpkqr.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gijhhnzdc.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gehmxsmzy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gnqlqsvst.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzxuxoss.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyodhxnt.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gpmgvpmfr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxqdvjoi.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gkpftfrur.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhpaferp.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprbvhnlq.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/guxvdhgbs.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzgptafn.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gutpgclyu.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gunslcbbl.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gwmsprrhr.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxtkabyl.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gxhzsvuje.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gudwcjogo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqoalcxm.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grreritdu.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gmehmejky.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxmqawmj.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwrpapst.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gsksqzlnn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhdjthjc.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gpmugjdpb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gkitlupge.sHtML


<!-- 参考信息 -->