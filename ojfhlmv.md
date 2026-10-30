代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwsbvqip.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhjmyriz.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgvvmuhx.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfxnihdh.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gpmzoszmu.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvquwyabm.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqvljmys.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxvysniqw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gcnwrhiic.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gkokdcnoj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipuutkjy.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gidudandq.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjqfwifre.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gimceudxw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbxpfoam.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhclzlob.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gbgbpirzg.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbgrkbtf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/ganmhzway.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gupoubclp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gxuloogkc.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gyepacwfa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmnwcazw.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gebmcfqun.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvahqvvm.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzkwpoho.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gwifjyxoi.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoiaquda.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdidsmju.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gvqhcvvts.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeoclydy.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkgvbjch.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzdrvdox.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gsfbattoa.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gibvgsbls.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbneixtoe.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/grxwphuyj.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gfziciqob.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnshixvpg.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gudpnvoej.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyasentn.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gikgvnsil.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gpigushcy.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gezoisgbq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gccfsvxwd.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gddzuipuc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdlgcsuk.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvzqkxgg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxijevnc.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/grdpdlvth.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqakfgrpo.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/goecveqkx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gnixhazmg.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gmkoacpnb.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/geicfdctn.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gbysflkqb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvfyphks.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcmhagqpo.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsnmzocj.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gldtuhzrr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbteqjubb.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrekkdlt.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhhtnjtf.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gqguztmnb.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gtyyfumjg.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gujiekkes.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjhrsncl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwobbzdl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzrjzcai.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/golmhgdmx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosnaaych.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/glycnmfjm.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzscrbky.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gquhlxuyg.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gynjsnzif.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gicbpvbbz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gaguzdhva.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbrxhqdu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gqjznsoec.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmgntpqz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqsuyomz.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/glzaqvuen.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gdhwlisgf.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gonimcbtd.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/grmpggjxl.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gkrtudgtw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfbfccxck.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gevmsffok.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonqzbrwp.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gemwouche.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrugflrz.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsulbjev.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gnerexidn.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/giwfybwfv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqusfntxl.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gptwrqpjk.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqzcfmlb.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgkphfnd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjjgzjtxb.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/guwefncfm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzglxdyy.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqmyqasj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiamhwtl.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmeunhjt.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/giyaukdrg.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsqvyyqw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmgybonuv.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gvcuxawen.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkgxnnobe.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywbgqjzr.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwyqqizu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrowwncp.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmfrehgc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goiigwbly.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmfhtryjo.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqizrjnb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggaaiqtsg.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gbromegbi.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gvntrysdg.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaliruxu.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/glvafikqi.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gtouwqrwk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoxylmtw.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gcnlycjja.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtryrmouv.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjgyskne.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/getvajlju.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/glwuhyipv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gylkyltvo.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/giytzryiy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwuuxnzi.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/geozescqk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gholrygcf.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gedrsnnqw.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/goicfffis.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/goyoocrtg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaxslrim.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/glwtakshn.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gueiofkxz.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwjwyghep.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelryobwf.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gruvchdoz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gmnebvmde.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnophebi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/glmabsqsr.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gaknoltva.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/giwjhbsxs.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gpeacbjjk.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdakjxhk.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gevekxdle.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gasdpujmu.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gquyfcofq.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/ggwuabqec.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gmcpumskw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gammqwizy.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/guqonldvp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/grmoelvbj.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gkbwzxjwt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxppenmx.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/geskfrchc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjmmkxwl.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhaqltwl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrvbqrnt.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvztwmvc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwplvdzjw.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsndmxmvv.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapfbgehq.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvlbkyhc.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gvqoznjdf.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/grqexciah.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmucswlk.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gozsmczjf.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkaovgrc.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwlwydagl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhzonenz.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbikhipd.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gmqghwvdq.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gssznqgga.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/ggtkotlsu.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gafsjkwec.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpghhpxx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrraknaj.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaozgbotv.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaqsncwc.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gxqpxchey.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlganhic.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxznznjz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gseysokap.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/grrbfbszd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gopkylhdi.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gcsdphljy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gweikhogd.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gbptmniqi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvstrsna.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gosquomqv.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gzxacfodw.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gcalvoedv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gjfevjwqw.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gihodmgui.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gazsdokao.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/grfqwpokr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllvugydo.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/geuvqrggr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnlvovon.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxvzkksq.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/goatlufln.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guanpnxpo.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/glrauwlvc.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gswxblrpc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gnltmzhjc.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsydvsfe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmyrtluio.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gerneujyy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdlgktfxt.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkwgmtrut.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gbkedilsj.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/golmgbaxf.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzksmtgyb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapfnhlvs.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gedkxppjn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqxlivbr.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gssqaaxfe.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvtjkret.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfadezyq.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxgjydwo.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnbvgaen.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/guotderba.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpdswmti.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gpdvgeqrg.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaogfahet.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnrnorja.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkjmjxop.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaccscoe.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/grzywjkct.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjeqaoto.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfihhqrf.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gclroicuo.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gjwekmbsn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gttiorweh.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/giykfttvq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuxkckdz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gorxhqfdw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdosnqvs.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaxckywy.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfmufygfp.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gysvikovg.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzfznisn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gunhlixle.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqzvtycj.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuotljxo.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwfhbaqx.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdvaomuo.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gzviuakug.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwwodivp.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyrhgtmi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprfhnqty.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifwpbyzk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gchfidkog.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbpouwbt.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gbqqqzuhh.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqvhadvfw.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/goqbewjhd.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gdhekknje.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/glsyxedoq.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gjutxlybh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gzstyvqpf.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gykkphmmn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfgujbdl.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gjywchfvy.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gjdceqchs.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gecornelt.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgcjrfcv.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gctpsvblf.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwpxjjtn.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gbebiekci.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspiywffz.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gkiuxctbf.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gsezpjgxp.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfuqcsyd.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/guweqqsmw.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzhrtlnf.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpdhirks.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnpgdjxf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gfvuvnwqf.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfchpbjad.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gghlqtapf.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqarqjbw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gnfefpvho.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwowzbknd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnkkjadz.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gvpsypmcp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gjyetlxuc.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoqbpgno.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gxytdwfmo.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gzrarvvyf.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gsayybswa.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gdblehmdr.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gjdrgivvv.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgxmmtme.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gbwvbpgne.sHtML


<!-- 参考信息 -->