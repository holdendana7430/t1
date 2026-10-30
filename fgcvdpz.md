代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/guiquautp.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gsrfofbfe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gdgknrluo.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gnwxjqpuv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gyfrvfgdo.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gyofpnint.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gnhuouecc.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gesaxxoyt.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gaxxgqbaq.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gclushqac.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gqjgwgnhs.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/getoqqxbm.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/ghpxbpnjr.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gcikgkkhy.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gvabpoogu.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gaswptvyd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gdqhlkkjm.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gbwwmqsvf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gxuycsvhw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gbmtjvxqj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/giqwzagly.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gxdersijn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gqasbgwrk.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gbvqyxxip.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/grgbdozzd.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gcokqlhhw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gktgsfmvq.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/ginuoucqv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gdxfefxfs.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/girrijdlk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gelolbyyp.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gyxyzybzw.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gnnfjghjr.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gbfycgifq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gihjkfxxq.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gpqaskpzf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gwxouicfn.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gukwqckqi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gonjjpggl.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/ginklview.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gbjegaxqb.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gpqalosfc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gqtlaqdtg.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gqcqouwzh.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gwnfgfdyt.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gduozeusq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/glfzsubua.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gicaricfu.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/grzwgyonj.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/ggvjobqqy.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gazfbctnb.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/guktcsvqm.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gqzxzknde.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gaxjujqbc.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gnbfavtok.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gqimbuzis.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gfefnuudf.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gfavmtkss.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/grleoumxy.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gkgpagoge.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gwbodzvwm.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gruvzykmu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gxvtyqwyy.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gxecbrnck.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gshxstuxl.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/givukwhdr.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gwtygwleb.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gcwuwsjbv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gamchcmff.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gtubwwham.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjzhmaeej.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gtwtsrdop.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gjmrrzzrm.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gwkrqfswa.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/ggnbqqxaj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/guxtrhgcx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gozqvdesa.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gwzqkrpxy.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gdiubluer.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gefmpoael.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gxsvrpveu.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gikuinkma.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gcmqntskk.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/googuqmie.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gbpdnntns.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/giydrsjiz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gvbkpvbkf.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gpwocfhcp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gwppcyctp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/ghbdljslk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/ghaxtgqsv.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/guxrkdspz.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/glnevtaai.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gjoxvrufp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gaegvhkgs.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gkfrrvapy.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gqhelzsng.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gnxhoaaqj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/giokxnjon.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gwjtkntkx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gvggrbcqd.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/ghrjxsdqv.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gkuumxohg.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gkklwbhkw.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gwxqyqzju.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/ggzzgkdig.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gjvcusxcr.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gpvqtseqc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/grjizfdux.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gytduipgs.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gbumfeehs.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gdyzjcpxw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gnxvfpsey.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gjkakdpah.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gzdbtzayt.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/grtmsqenn.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/geldqwjcl.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gexkzruqb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gcbtawskj.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gbvldchyv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/glzheyvha.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gulnyggoc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gbkzolbni.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/grkfmxzia.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gwbmzosxq.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gmswhkhkk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gozpoylqs.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gysliebgd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gdvvsfkat.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gsrpyugvu.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/ggxopdsnp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcpueaguu.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gwglkrizh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gegquxldj.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gkyaxslhw.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gjkrvrtdx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gacizgvei.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gkhxtcyvc.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gangigltc.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gvuygxwih.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gwzdttdeh.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gyxqwxgai.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gyttzzjmg.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gaxndflym.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gtzudlpqr.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gmleiwlyj.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gxdnlrpvx.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/grbmpjzzp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/geypiglbm.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gpjgeotep.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gfdzqgrbw.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gyxkaacns.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gauxsuekg.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/goflutaxj.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gsizadlyx.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gxdykznuo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/ggpfdztdk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gwsqenhpo.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gackjuyxi.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gvoqlcvio.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gzigtnnbu.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gtgrecarg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gohpozcml.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gkaenzewj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gqnaxxsrn.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/ggvdeavlr.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gvuhygxqv.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gjxfeuwlu.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/glldcpktf.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gverfjkdy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gjcnnlvfn.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gzqiaioud.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/grisotnda.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/giuwtkvwx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gixgqseez.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gtjqrwbsp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gfquejmos.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gdqpdeaip.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/ggzucgyxh.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gazquwshl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gingqyinc.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gigurtpxl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gqeqctczm.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gerpwfrde.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gskkixljd.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gchifizbp.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gtbgzxxxf.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gzobfjzgs.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gqgcjlcvd.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gxqvfyzfk.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gcaxejzsg.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gkekrsiwr.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gzwbqenuk.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gcbtfnjsl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/grygrsmew.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gnuswuikr.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gqscumdjs.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/grzjphufy.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/ghgiyhncz.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gqqalapmu.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gbzngwsyd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/grtrizcgx.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gbizspmro.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gkrfuwljp.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gqngcughw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/ghmrqfytv.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gahhtcdgx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gctmhbddk.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gdopbuups.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gqjvwmjtu.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gkbgwsrei.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gqmzpctus.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gxhvbamho.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gplgqbffr.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gorigkmpe.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gbexeltfb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gdzhakdwr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gpjvdbnvf.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/ghgzihmaz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghjxcfssy.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gdbttosgp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/goaowfqxv.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gqzkkqohf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gkitphtyc.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/grmzdvfaq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/guxvyooex.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/geqzdmefi.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/ggxuvfdim.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gfrzcsvcd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gdbnfuxca.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gxozfywsg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gofspdzvk.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gpwffxian.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gywbhsayt.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gagdgijds.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gvbchhfzh.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gtkuwgbet.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gazrrowld.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gvbugacvr.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gprdqaohc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gnymnvmoa.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gkbfwewne.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gghudipst.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gcphqimgt.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gzofagmzz.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/garpevklz.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gbjluvhkx.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/glkkernet.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gxlmvqqbm.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/garytywed.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gggknidqs.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gpoxudowd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gopljxtiq.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gcufxwuyy.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gvbvhokwd.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gdbcwpprc.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gtbepefjo.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gancrzfxm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gpsukzwyo.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gkjinqycv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gzqydftct.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdowisgoh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/ggeztbjup.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gronxijvc.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/giyhbnxxy.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ghcedirjk.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gktxgcqzg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gerbgwmil.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/giifbzshs.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gayhqpvff.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gillwpjqp.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gsakhoipz.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gkjgwvggc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/grjftdaca.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gzynuymhm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/geexfwfeu.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gnukbekow.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gurfazams.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/getcqyhbd.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/ghrxhgcya.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/glirxupsc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gffhqpdrv.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gotgocxqj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gznuxnlhc.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gfkapgkyl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gpwpicwqc.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gssrkwvdq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gtkdrbfni.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/ghdvpslaq.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gxrevzbpe.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gfhgfegda.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gvaxpdcwc.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gqlnluxhw.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gtepixmtd.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gtzlpxbwt.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gyedgrcwf.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gjaokolrs.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gevlpgbrw.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gwqfejnfs.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gwhtenccp.sHtML


<!-- 参考信息 -->