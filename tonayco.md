代发 wailian999

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/grrpaxxrn.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gjmgdbwak.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gazdalkgk.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gtepuxcmz.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gzybtkqtx.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gmywchzmn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gqaifevpt.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gsrnunwrm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gbppxyzvt.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gxzgpegsq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gmsysqzbq.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gkvixfads.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gdfqsczmx.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gyiiyyxux.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/ghumzeecq.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/ghxdaskcl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gtremrqvz.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gtsfrghhu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/guovqhplt.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gqghackxt.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gyxmbkrqx.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gfpighpcd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/grevyqztk.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gwccjluse.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gypnhcxnt.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gahrwkgcn.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/glcttpnuv.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gdguryjoc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gmyvjpbjp.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gazmwngxi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gpjcelzkw.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gyhgelind.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gxmtchjag.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gzrxtxnei.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gxkyqbbap.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gesxtcvqw.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gbsqhvmyy.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gzwzmvltn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gngsigoxi.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gdpdufala.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gbqjwijqh.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gmsnzixrn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gpedbtqsd.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gghciqhzm.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gdacnadjt.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gzxoawixq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gvntiyoec.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gucakcuub.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/goeonytmr.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gaecrbaap.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gthbzjpml.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/grijtuxkn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gvoxvczbq.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gkbmwhbeg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gfqsytqge.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gttizrhrm.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/ghojqxiss.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/ggdseztmt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gufhwdiiu.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gaibwawmc.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gwzbmogmw.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gqmhumbwo.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gntaudtdi.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gdcgfkwoj.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gujxhouhf.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gzutcfzvk.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gfrdhuoxs.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gcyyfkxoq.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gfxxnwfex.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gyislrcce.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/godkhxblj.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gdilxehvd.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gwkmzytyv.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/guyqnyaut.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gjivwikrc.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gsehezeyg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gzrnmfktw.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gboufocxm.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gqzthwzeu.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gzwuylxye.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gdcjoqyam.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/grnqwpuuw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/ghyoummzn.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/grqlhmdts.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gtrmddrdp.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gkcvdrohy.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gjzbopjwo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gbvyhhiqg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gnhozygoe.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gpurjsfzp.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gqkcybpiq.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gtwexuwdm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gntxlqjgi.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gpwxcvpga.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gpogcitze.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gydgilaan.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gkscizble.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/ghfxvbkka.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gneyxpsdr.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gquspgxzl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gvrrasmis.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gxubyxbrg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/ghzplijdk.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gikqkbdls.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gbxxtcsba.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gtqbwubhn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gdneochiw.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gsnkexuig.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gurdzqnqq.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gxdqcqyll.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/galljocmb.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gjakpwmsl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gkzduzjev.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gibjhxvvc.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gkhndmkfk.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/ghnppsctu.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gukkwpxcc.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gwycjrhxs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gotbeiwah.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gcahsezns.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gmsnxqjmq.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gvjctbqsq.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gfxuizzes.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gzqxjmqgp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/guzthlkit.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gnogjifmg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gapvvaskz.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gvhqnllvf.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gbmoybtgb.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gfcojzunq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gqetrdvka.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gcritutbu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gsizekxeb.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gtmjousfi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gmbgmjbar.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gbintcnrv.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gekmivdwa.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gmddstrdc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/goyedvnhb.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gzpczprch.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gtxxwilqf.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gkkajjjgy.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gutxjnykp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxmmcptzs.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gpuoavril.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyvjyztba.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gbmmryksj.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gyqovozco.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/glzeevxev.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gfrvckqyy.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/glvuydwzr.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gcvncfbtq.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gerqjuoaz.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gvtrlpdde.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/ghwptzfya.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gbqocmyot.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gfqtribja.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gicgutowh.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/ghlpuduub.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gfalghiec.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/ghkpdigjb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gtmcocsgr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gytivpvhb.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/grinpnyrb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gobvprhwl.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gyeeslmkz.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gdxsvwqxx.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gyeaizrhb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gagcnnvhu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gedaazlez.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gcdctiige.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gierfmsfk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gcjjmnnxe.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gipvttguf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gjccofhrf.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gzlpvsrsd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gybvvipdf.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/giymwybfo.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gukvmuijw.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gayfcxzwi.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/glzpbpori.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gfubxkrgr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gkjfrmkck.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gosjgierz.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gexmyapkn.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gszhbsydl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/ggzlgouvh.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gfridhzjl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gqwyqmwvn.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gypciivhg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gxuqmrsxv.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gmgognhkk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/godunuxcn.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gdfumbsip.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/grkbxrmha.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gfwuavhuu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gxwezpfls.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gpymhvmkm.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/grscmnikb.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gcmcnsehk.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gicknmsuk.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/ggiduedqu.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gtbeabbcs.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gyeashaev.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gvdlgfnkb.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gtudwnkwu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gkjgtkpxr.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gckyhzxlg.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/ghhevomxh.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/geobiiuhf.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/ggkvverxs.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/glrjidzhx.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/ggpikudjs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gidqrlptx.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gapieeyqv.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gwdtpdlpq.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gxprzbncn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gdtppkxwc.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gdenmqjeb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gqvtxzbef.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gmwfkvxde.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gnbantauo.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gletflvfe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gjrdfdkqs.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/guhyjgddg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gqlsparfx.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gdxvnbvmw.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gmnzrklsi.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gjbumukbg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gdlsdcfib.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gpbrtdcff.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gybzyutsc.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gtspudhuh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gdewhzwsx.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gqjtdqzwd.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gkskiidgk.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gzfheopgo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/ghgrxpvib.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gqbibqnxv.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/ghxjlmimw.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gglcyfhwy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gxuiubska.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gxtgqjkhs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gounhwbwp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gyevikvdt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gdckqvwot.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gfajsqjgs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/goivjcrps.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gjgdhpoie.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gfeplgwje.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gfuutbvow.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/grvzhymwf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gbnrylsya.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gzfcsbjlh.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gxsdkbpon.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gbvihxule.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gnlgjtskj.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gipvaennr.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/ghzjgvdmw.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gbayoiumy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gnbwkvpzv.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gjphecnre.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gsbzsuwut.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/glygmsqvj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gdpkivxnj.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gnabwfqrs.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gwnxvjyvc.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/girzvueoh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/garkjjmcf.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gxonvsghl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gvdhmzmgz.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gkavaqioc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gpgdgjkru.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvwmvkyzn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gcrpkrnxs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdabaurib.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gajvojyrw.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gvaeonsfz.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gjgprpnru.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gfbepgjpu.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gdmlwokmj.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/ggehxfhxy.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gptzietzo.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gbhyvgadm.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gtxwjcefa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gnbwkydwp.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gzhylsokv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gwbnkbqbw.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gkcbeosll.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gsbftnbgo.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gmnjudhao.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gcobaszty.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gimllxjeu.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/ggbtaaetz.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/glkcrvofi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gghysovtc.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gtdcxjxdp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gqndvzfjz.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gqhvkahby.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/geusjhoje.sHtML


<!-- 参考信息 -->