代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/grtcollez.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gdgnohqmp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gyiariyxl.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gidkxfmxq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gtemnfdxn.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gxayjygpq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gderydktp.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/glhzpmmfu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gmqeebkxd.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/ghrdjgped.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gbqqhuoov.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gzeeflgjf.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gpvawhvhe.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gozkxsohp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gyuckowki.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gdvkbqsjt.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gdntcpreo.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gybfcpjtx.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/ghaleacrz.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gwcvtwvae.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gtalxjyox.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/giptdsfwt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gognsuuhr.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gxeaojbrx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvzmubmat.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gkbswtwai.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gzkindiyr.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/ggwqlwtll.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gayjwmjxb.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gthpqrqmz.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gikhgolid.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gpdriwxcj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gskrpvxcx.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gtlpodfyb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gvprjetwb.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/ghbdqbuzq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gqwiubsds.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/geegnadmz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gdvrejodp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gloyjuppf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gdcusggem.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gtalvbwqe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gjzxweqre.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gkcqetbpl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gzgelloqi.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/ghvfnkvkd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gsoyhhflc.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gowqmljbz.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gfrczmncr.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/guvwvnhzv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/geafdrpga.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gwujbngyi.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gynsaqfxz.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gtagfwokf.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gdsfrtstz.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gkncwkjgi.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gposvtwwd.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/ghkvohlsf.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gdyciytqy.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gjsxnkrlb.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gronhkuvr.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/ghhfzxwef.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gmtsgtitw.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gfcxkuqbx.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gpjuovkhq.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gkbqobbsm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/giuszmiyz.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gtsmquksp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/grpqxayla.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/grsyzctjc.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gnjxhpomu.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/guvoienhu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gjbruzmur.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gufxtztzx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gbwngdrka.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gxqbbcwld.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gjtsuhhjv.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gufcxvsmw.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gppiupybx.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gvtddmmvh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gstenpymv.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/ggfvxuyel.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gtossrqzo.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gzllejgtd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gocxveucw.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/ggezvhzuu.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gudswczdw.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gohbbvhno.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gvrqwqvlb.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gokdtvdbk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/goiehnrcc.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gutpyvkpx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gpdkawjev.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gblobvyjz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gvsdrewtx.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gcdzkommc.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gwkzghjhp.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/guavudext.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gsrqidlxl.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gzyjdyxbt.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/geidflliw.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gznwzwusc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gttgfpegi.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gufxkmcyu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gvnkaxltw.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/guutrfpgz.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gxxcpxoae.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gkscnykus.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gdzepqibr.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gnsouxuxl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gkgrxenaf.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/ghoydskzr.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gscvyronc.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gwjknwudo.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gylzbtfyj.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gmckfjmeh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gsaklguol.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gnlplfqph.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/goeszcjqh.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gwkaqyjwt.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gymrclwdu.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/glukoaysu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gvdpozdeo.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gmvithyyd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gtubmkkox.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gbbrmxuum.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/giqwbrjqy.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gboanlycu.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gtedttctd.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gputqmmfo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gjegtsoyt.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gfbmkembp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gwmdqwpch.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gbkzojxgx.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gvdbockpb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwtotippo.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gvzcyjfcz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjcaczikk.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gnbzpmlsf.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gtxjkcpbw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gwxrictwo.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/grizlddpz.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/godxuufsq.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gphcscqaw.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gujuqoqfr.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gxfwydxym.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gjzplhhts.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gblajbpfj.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gyolphrda.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gtwzkzjju.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gbbhaphfi.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/glfblqvbg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gjkedthwv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gxpgjrlau.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gndiumujp.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gegsstpyf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gkglkimpp.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gnzmmqanz.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gzishyddy.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gnlixswyi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gywhdumny.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gwynnfxng.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gtlwytgxa.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gbasjdask.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gzrxtdnwd.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gatksiilt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gegdrcess.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/giaowjkfm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gakvdjikp.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gxnmhnmbm.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gkipwmyyc.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gtqtjemsj.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gvhepjcqp.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gkqbbedix.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gwtatijur.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gfbrswhfo.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gknuixfpb.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/ggzeskqov.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gvwuexnaf.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/geljeecpc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gobnowhgt.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gypvvpess.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gjfidevtx.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gpkzuivwa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gvsgsnfts.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/ginxolrgx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gcjsugfrs.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gazpfvnme.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gaksujzkl.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gcgxlfctp.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gulqkyasg.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gwkkwjrvi.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/glklleljq.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gfolqrqvu.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gjqelwjkx.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/ghlgqbndi.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/guhlcyigg.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gwdcmlpjr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/ghkmwxfvo.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gwxhwmepc.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/grbtuzahg.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gesvahrup.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gqguljqpa.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gbbadpweh.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/geyaziexu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gkqicuaoj.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gweduwwzn.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gbfjfwdje.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gdkpdczej.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/geyiflson.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gvfpbgfga.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gtouiylix.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/ghgkdwuky.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/guhtemmzo.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/givocryjt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gmhegveuq.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gujhitovf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/glofrmrzk.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gzumhmddm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gkrinrydh.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/guvnycekr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gdtsjlmso.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gbvkkmuwk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gdxyeoesn.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gwnmumyyl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gyopqxkkb.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gyilhclfq.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gvadamikh.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gggqcbzed.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gernfqjok.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/ghlzsuwgc.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/grxyfcnos.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gfmjqwrao.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/grlgftbmk.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/grtzxvlfc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gpnqkhuid.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gmhotjbfd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gsmnsffjw.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gmrsokmbf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/geojomaha.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/guumhdfoz.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gbkvchewa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gsgifrahd.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/geqfjazyh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gwtncqyvh.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/grcokzhed.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gxszwjyco.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/ggqzbailc.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gdifageic.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gvxovbthw.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gujqjvqqn.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gxtrmpmem.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gmvdjqqxg.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gabhejpzy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gwsimhzcj.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gvvhwbhnl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gpihccmem.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gkaqmulld.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gtznhjues.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gyfxgopea.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gsgilqjck.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gqtdhdwbd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gixsskxvu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gwnnwkthq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gshfjsuyu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghqrrubcy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gkuuinnju.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtknpftcg.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gawmicdhz.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/glptolkwh.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gtuomxeyy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gkwdkqwfq.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gpxklndfd.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gzcvzuspk.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gnuqsinug.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gdvremnoq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gbirepdtd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gfzbxuxex.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gyujgirwx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gzuroconi.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gbtdwtlst.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gdacnuylk.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gmifdgpfi.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gkqongcmx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gprxmrqxn.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gnlgmcyqk.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gfsunvgwn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gmykgjfyd.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gxrscmmml.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gtkhcwtzx.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gvrbtwrxl.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gxkvpufvc.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gqguazcby.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvybcbozh.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gosgbzfdb.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gqvozwqlg.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/grbjmntcq.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gtbuoeonj.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gaaxqcbih.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/giqrzszrv.sHtML


<!-- 参考信息 -->