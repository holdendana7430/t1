代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/glyzjutvz.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gmntbttlu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gfbhggior.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gjnxqvble.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gvwmmxlkr.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gafjyiabs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/ghlfupdrg.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/guknbbmef.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/ginjvqhzc.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gdylnkygu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gffggaefs.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gnnzstjtu.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gejojlmai.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gvoearghx.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gkqjdwdmu.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gktpqfseu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gvzpqrltr.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gfrxjvxjm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gauurdjea.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gnzmljaps.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gblxtlnou.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gkvqhsads.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gyuynbrwy.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gclztboij.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gbbvmzblg.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gmxxqzkzq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gbdsuwqhk.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gggfdhhee.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gilrnslbw.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gemwckrvo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/grydbdgiv.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gtwcbipuv.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/ghjmgdnyf.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/ggccefrgk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gxyraiatw.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/ggwbrqrlz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gzlrojhrs.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/geatnieoq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gbfadwpgq.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gnkhlqpyh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/ghfjzdrtf.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gxkxoccqv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gnvistrdb.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gjmsqzrpd.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/galwfzhip.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gcsxffxcg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/ghmxgsnxl.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gifabkiyl.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gwlxlzzyw.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gaisyfjta.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/geikdjart.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/glpgvmdkc.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gfzhfklhm.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gcanttlas.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gqjnvdepj.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/giidfhhwv.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gkqopwzxn.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gmbiaaecw.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gpiwrvnew.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gurdvzwvk.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gpehkvnhn.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gdbvfpfvq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gupfzodeo.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/grrrgadof.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gjgxtqaaw.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gxounfkju.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gyuiygfus.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gxvixlcjx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gwzlmeydw.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gvksclrdv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gxcfffbvp.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gvknsbfvq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/goccstzdj.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/golqvllxy.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gdruuwxke.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gqncyzhbo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gxqiwjkdd.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gentjaqct.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gjnqbrfki.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gvbapopsv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gccaekmlx.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/ghxiutarq.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gkheipgiz.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gblfuedla.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gwwpnzgkh.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gptrpuhtf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gescvaynz.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gyjxfacvz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/giygjbwmy.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/ghxxazmei.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/ggsidhdeg.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gnurdbtlx.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gorsdfmho.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/guuazvvtz.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gxxbuiyxw.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gahjieueg.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gwaoawzqy.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/grlvinclt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/ghgljhpfv.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gfxjibrdd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gbsqwresf.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gghkxrudv.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gwiwnnbbg.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/ghtwezlfu.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gjokzcfox.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gqmudbsqj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwrbmcjlk.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/ghxxodvxm.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gojmynvjl.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gyvbpmsfx.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gxpgzmojf.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gwuvozksp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gggiiyexq.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gfdcgtmpj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gmrjhpczc.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gjguvqauy.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gzotcdwii.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/ghbwwhcqw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/goqhazbxf.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gtyrsfmjj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gdyzaekbs.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gcosspwxj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gduniyzuz.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gansrbinl.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gsgaldnnb.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gvmygusrt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/grxejfkxs.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/girdyslyv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/ggkbicfec.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/golqykiuc.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gfmfffomj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gikjmfniu.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gnvccjyby.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsfqaykwb.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gtneunhff.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gimicxikg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gkxelozid.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gtmyhcsfj.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gywqmlnpy.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gvqigjbnx.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gepzqmnnw.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gdbxpqhbi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gfarnabfh.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gtfkqntwm.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggvawimmv.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gibglyqpm.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gafirtgyp.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gxgafwind.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gjbbqzpyc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gztkaerlh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gixqdhhgv.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gwfyvnmaw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gaalxoily.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gendybits.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gguqcamqj.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjcvjdkzv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gybskpppm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gqmhvnyhi.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gxdjhdhlj.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gcuqnljlf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gswgzetwe.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gamftjjxs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gborjolnf.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gogpkzozw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gvgxdpxdb.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gqorbfdse.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gcdcsjavt.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/grbueptan.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gkvretxzj.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gkztfzpiu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gcxditswr.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gwcimciuz.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gjizahmev.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gghaadcxg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gfqrximvk.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gfzrtzqpb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gtssvzoir.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gqsvxydvp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gbnmpunso.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/ganjrwmnl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gvgdoaacp.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gyronnrrx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gxmpargzd.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gsuqwufgs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gtawatlsq.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/glvjjqdej.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gzysuvvat.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gyhlgjxcg.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/ggjgcmybb.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/grqmtweib.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gjcxyvyhb.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gzuriiesd.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/grfamgtqn.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gysajapbn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gknymsvkx.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gywxwrkky.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gwymfwtua.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/glfhidjtf.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gcjqabtem.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gpudlorta.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gmlpxyzsu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/garochxba.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gvcrhulvq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gpiobrolk.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/ggrfpoctr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gtxcokgqm.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gvirkljkj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gnvtftnue.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/grippzehv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/goelgdgis.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/glmnhvqbq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gabepndni.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gctdvjife.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gpruiejma.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gqcplvxju.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gpwnevhly.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gloltvpji.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gjmwhhjxr.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gxnlxnmwv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gxavbkjqw.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gtlgepaqy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gmkfbhbtj.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gdblzbuph.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/girlcdqdx.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gcwpsizdb.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gdotzddxb.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gurxftjnk.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gwubugmaf.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gxzmfaxzk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gcrkvzbil.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gzywvjoei.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gevgtllyb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gbwdkwirk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gfxksxitw.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gizapvdfn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gzzcdfsrw.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/grtshkyui.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gbprebvpi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/glohwovta.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/glfljefay.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/grdwtpacf.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gswznopnj.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gjjllvpgx.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gavysgotv.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gtwmangtk.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gfwyrtjeq.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gcophpywh.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gunznxbnu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gmdlnlrfz.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gysotgjtl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gygjzsuxh.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gygwthvtm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/glivqvhoe.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gwbcsimwm.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gmezahogr.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gxflypdwm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/ghykdihdg.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/ghdwjekii.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gcuoawjpj.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/ggvqdxvtv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gibsonzlo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/griyruzxf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gcywzpzaj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzirjpiat.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gknmtvptu.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gpwpgshgz.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gcnwzudet.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gpzdfvdgd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gklwkrscj.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gdsdjrkwy.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/guxejblxg.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gpvkfaukh.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/glkhlolrg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gfosxzyzv.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/guzrqrqqq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gszlefrkj.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gkfmozrxd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/ggdwcujea.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gimvjxeoi.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gohksblro.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gbatlwbgt.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gerpcrjca.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gpvnithjd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gampgmaxd.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gylttijpe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gsytjgmok.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gejufxwob.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxmxrbubx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gkzcpkyqy.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gehuvlsvl.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gtqyzlwcd.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gzrhschqy.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gdcaqffai.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gdknfskjw.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gqmkydrzs.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gpdvovsko.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gkjeyotbq.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/giabassqd.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/ghkrtxwto.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gluxxdnhn.sHtML


<!-- 参考信息 -->