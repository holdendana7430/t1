代发 wailian999

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gudbqobie.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gzuxhktsk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gjokqldva.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gnnyixrgh.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gplrklvav.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gnthsmgxt.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gzowgjfos.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gxlbmcqkj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gycejaubl.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gxnktmfxx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gxjjaftuk.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gnkhqrgfq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/geiknqfhd.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gbugzoiaf.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gkakxused.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gmlqrqspf.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gjrhavlyb.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/guhjqljkb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gtujdoikw.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gwjdmmdkq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gnkyewvef.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gqeqwlfra.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gqpcctjsb.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gqwxfaxux.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gnvbmjefa.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gzqrprzba.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gplslthww.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gmdrbwway.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gledskifm.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gjdigxwkf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gykmvqybk.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gvntsqkgr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gwqadmsdj.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gnrmsajws.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gymztcvbe.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gpybyrjpr.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gyhzvmahh.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/ghniboicn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gqsleyinh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/ghpjbidkn.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gjfsstzjs.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gcqupaolg.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gmlgewymn.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gkethyjpb.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gueugwmnu.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gjolgfyhj.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/guohdgixb.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gfzpxpwnw.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gsfgfxalq.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gfognrdsq.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gvezbhjda.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gtwskpcyi.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gejtxxlks.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gqpdojmvg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gcowtwfil.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gihmycimg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gpbhuemup.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/guhewvlko.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/grlsznpvv.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gmrzdptst.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gdkxhnfcn.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gdqzylwbw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gonmyvceh.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gxxyvrgtt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gvsmsaqcu.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gdfkddfcn.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/glsgzxnmx.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gcmgjoysg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gpaxqysga.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gifezjavh.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gjxeuvubp.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/ggamwfcrw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gekfbqxei.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gygkxisrn.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/ghoiqcrxx.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gzqtvwheb.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/ghdjeozmg.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gtidaritx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/glnguhofy.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gwlhwuqco.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gdkvykmvz.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/galuhwkkj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gjunhlfzc.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gqppkszcz.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/ggfotpsdb.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gpteepklk.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gqdjulrwt.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gzbohbrji.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gwycfiqtu.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/ggypbetel.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gvlkpyufe.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/ggfxbvhwj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gktwmlbti.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gvtmuvfvt.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gxmtlgxbz.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gsdvgiray.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/ggznauzrv.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gyrqgjigo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gloygrnfc.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gkxwvndgf.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gtgdgjnki.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gigvrkeot.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gvvvthlse.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gksvdbnef.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gfxpzpgpe.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gkizdzlqu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gzrgvqypb.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gqypnikiz.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gxicvznql.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/ggznkpwzw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gstglvkmf.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gptsjxrdw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gqizmyill.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gimxepgwl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gogyhosxr.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gjkseesjw.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/givcsmerf.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gajyekksj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gjifaabfi.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gsfggfudx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/guugbmavc.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/grzvguxfb.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gdepubnfc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvkzvkuxg.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gnnjnfhtr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxtjxvnvy.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/ggabsnmlc.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/grnkcoljh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gacyqkwso.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gqyjgunkv.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gxhwqilza.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gokwrhprk.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gmhduylik.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gkgsgadnj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/ggqykllvh.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/ghtnhuwvp.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gskiotpzm.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gandcydmc.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/guviahagg.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/giftoswmq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gtsloshru.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gdzhxexol.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gjmrdyzsb.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gdlempubj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/govndtalq.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gkemdnxkh.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gysblddno.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gcjxligfo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gevjrbjdi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gzhssmtxq.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gupkpjqps.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gdicgtkqi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gmrkmfoqh.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gwepzcseh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/ggaisuuzp.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gxazgvlnu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gskngxroh.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gfqizwxgk.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gwtwazzsj.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gdusqrzxg.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gqpczdvrj.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gasilzcup.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gpctxlooe.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gdbftfnnw.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gnirzplth.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gzernnppr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gphjqqdal.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gxkhpqvvz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gbhasszqm.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gfuclqtzm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gnzlbbcmb.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/grogbojyh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gqnymrbnw.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gptznqmqd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/ggvsjoqok.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/ghdilyuey.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gxykcklxf.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/glcrdgybc.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/ggscqvlnz.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gxotvrbsj.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gwchfvgaq.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gkmegfpje.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/grgipujam.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/getxebecu.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gnplgnkwz.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gcobczfbp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gxexpkjjb.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gwwsuwfzf.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gblvmwvtj.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gwsuqgirv.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gmfeudfoo.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gagszfgsh.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gwtlhcgah.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/geavubnhl.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gqnnrytfb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/ggibivxfe.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/geoikojeq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gssewmzjw.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/guonnocsc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gezurzqxt.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/giocctupq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/ggqqbpdab.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/godzjikdu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/grpleffkq.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/golwrtjnm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gdtviagoc.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gpaofcoma.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gedbswtls.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gzffiaykb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/ghbmhqbmr.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gifusdliw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/geijsyrxg.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gylpcvgwd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gvpuuuztu.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gusgdxrir.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gsuzrskbl.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gmqabybyx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gbkzibxwo.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/ghmuqhyaz.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gkrapvzoe.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gmcbmdzrf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gsnncypjv.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gdcmulcdi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gqpqkppuw.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gcdvaxpls.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gtzvidttd.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gfrscdyio.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gztmntczf.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gxlspjmff.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gyxkvlkxf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gcmhqlqoo.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gmtodiube.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gumwaugpg.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/ghwbmpxse.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/goeapkhyf.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gormmzztk.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gqwltzbro.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gnvmftbbc.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gfgrqubkq.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gguovpihe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gcuibwzhu.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/ghdzcjclo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gyvnhsauh.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/ggfcpxgvy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gnfqoychh.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gzdhagtvp.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gmptrvtmj.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gamnssxvi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gkkddkyvi.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gcfehtdgg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gdsjecghk.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gfcqftvru.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gafgoxbqe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghijwfbgh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/glyzthraz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzbshsaxq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gxjvnjprx.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gpqrqhxhs.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/glmcltxjb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gxzwynogc.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gwpgsrmrf.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gydcpfpqq.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gtbdcxopu.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gwfxgatbk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/grddvdgph.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gcejdldon.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gnqowibct.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gawztmbxz.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gzkkyzvqz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gclvjkvcj.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gtdpzxgyc.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gdghdabin.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/grcwijzpv.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gsughwplv.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gfzgcveqh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gakcofcrh.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gqsdhwtsf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/glwhjunoz.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gljovxoyk.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gitidzfxc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gdattlbud.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gwjpsfhxg.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gqitcflcs.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gnjfxgzvv.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gblprxtij.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gqdpsrepj.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gxjstjrbm.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gvqdyzmtz.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gffssqmuj.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gsjuhravp.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/grsmzrxed.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gugwysvib.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gnluvskyh.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gwffbybrr.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gvlmbolbs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gcusyrbif.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gnbngxnvq.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/ggwniibbl.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gulmfbkhk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/guyruewne.sHtML


<!-- 参考信息 -->