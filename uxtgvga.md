代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzqcyuqao.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gmxrhwdbz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gjenkiynf.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gmciysazd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gjpqztulo.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gflxjobtw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/giminjprs.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/giegubvuf.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gqidymzyo.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gtgcppnhl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/ggwcedyeo.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gctmvdbmh.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gcjxjbpig.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gbsueuqsi.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gggectfer.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/ggbfsecaa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/guogtqodr.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gjsjryyft.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/ggqpjhhyf.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gbnybopae.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gxhavberl.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/ghasvjtey.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gmomremtc.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gvxhawnql.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gjdltuagt.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gwpwkistp.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gahrmedsk.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gtiatwpll.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gmgotoqhh.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gobyddnwe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gskyyddvy.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gtlvudztu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gynhrryus.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gzcpystur.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gjarpkvdo.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gghckzdlp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gvunqewzm.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gmohwzpxc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gzjaqspak.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gtdsdpegv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gpqgovyzv.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/grihvowkf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gwoluvfnv.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/grkcrbfed.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gllhkkwrx.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gslyudtlq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/goydqngxq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gpfscbdrp.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gspfyctul.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/ghuwugdho.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gnczhnqkg.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/ghdabsljn.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/ggdbhtspo.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gzgecsblz.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gticqqyop.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gotifqucn.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gxsifwgjj.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/glvavmqel.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gwyxwlqga.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/grcbqwfmz.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/ghztfxzou.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gisqxewjs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gmbusasdj.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/ggnmchtlz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gbgzhjwfw.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gznoqekfd.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gkhbmpgme.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gsqpcjsmp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gudyauehj.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gennperos.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/ggrvelyxc.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/ggvuxjbaf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gwrayvhsy.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gbdqmkraf.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gnsdkwdhf.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/grhecmxfr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/ggbiysnlb.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/grfutpojm.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gfmwtqaxs.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gosbqqeti.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gtjmxvbrr.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/ghtuxvtmm.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gfdukooem.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gitverwom.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gqwqjrary.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gkgvfhzfd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/guebvbknd.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gxtfjfszp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gpnxjasnh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gnpqrwglz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gyxybrxpd.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gsgblqmxt.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gwuiurvxo.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gnekqygkw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gywrxdtya.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gexpykftn.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gsegiksfo.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gjbizxlpz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/goislirho.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/guggxwsgh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gvnbvitaf.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/grdxczknc.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gtfjmivbu.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/glvrmxgtg.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gqynijnmr.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gozrqndaq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gtpolrevp.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gmmcsqdft.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gnbrrddek.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gefxniieg.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gzacopqrk.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gsdomwapc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gbscbvuzl.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gnrmlmqzm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gkjpzvpuw.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gzejblgvm.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gibpnjsnt.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gxdssainz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gooltoovt.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gelzlaztf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gxjljgkfo.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gckdxewyy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gfzlpbdrr.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/ginokywhz.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gawfkpxoi.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/grwwxopnd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gegfpapzy.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gktgwviea.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gfdwnxaki.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gyaebwitb.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gzfvflsuc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gstmizghk.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/guxcwbomf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gflzztfec.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gtrwcptun.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gyxmkysud.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gwseprrjq.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gciypiyvh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gbdjtdtmu.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gpwoeugvm.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gbybajfsg.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gspkwmmag.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gufqvrwcj.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/ghiglycck.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gyczdtjjw.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gzwkujlat.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gyyepwjpr.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gdjwrvanh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gbivftwjr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gbhxdcvqy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gqtoojtpk.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gajznbdki.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/ggavbxvla.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gwcputkdf.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gpgaewjsp.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/glsfnrksg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gyfryihjo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/glkhvmqad.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gvrxggljy.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gurwsoecj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gpxvzxdel.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/ghbfqhaex.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gkofmzzhr.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gbmobydzj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gsfahjzth.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gubdwfbqj.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gxfnzjfax.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gyqpxgzjj.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/ggkkhqkhp.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gubigmvjn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/ghzorddrf.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gjcmlodht.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gzazhyjts.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/ggkkkxutu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gykdbjzyi.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gbnupgvvy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/grstwxaab.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gggmmxuub.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gomselwqx.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gmvwuoivd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/ghlyrpdcw.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gwycwfpkw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gvwqcbafw.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gbjmrnowc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gbnhaoreb.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gveiulksn.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gbimhclpj.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/ggblpdtnu.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gchjqwyij.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/grqiszhvy.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gyzqrjrnt.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gixhtkbjz.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/giolvowqb.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gaxgbgfir.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/glcwaqpud.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gqeflktjk.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gqqaxbbvi.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/giosmoqyy.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gdtryzpyv.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gftrbuexg.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/ghizyzjcd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gzwctpppw.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gddlmxuki.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gxqwfrzzm.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gexkmkgvi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gshezlcuy.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gipujdgle.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/giiidwdhu.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gctxuysev.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gygxotzok.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gstayilxd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gvvdepwvk.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/guxauddxf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/giilgpwnb.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gfrqgxqei.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gusqtopbj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gwwihupfy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gxrccfkxm.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/ghzcauoag.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gnnavgjvr.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gefutgkxt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gkxejtwfg.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gosdggjau.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gwirhimcn.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gnlpmkxni.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gbdaxnwto.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gsgwzxbay.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gittjggtk.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gabxnjobd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gnncxtxfo.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gxeymoyyk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/glyjhbtom.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gdblfsyna.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/ghlykhouf.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gaahqdvnl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/ghvvdvelj.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/ggbhumaiu.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/guamsssrj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gulaiqaec.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gptuycnbj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gkvofwjvm.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/ghsnzlmxy.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gvgscattt.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/grmxhctdd.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gymqzldxd.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gqfetsoyq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gatgjvzdz.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gjfwejmke.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gfyxpanuo.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gfnezhgtd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gajzlojyn.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gzuhnnrkp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gmnfhddpe.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gcavtbbqr.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gcyztaell.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gqtakuxtl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gonmqqjcy.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gqowyqghf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gbgovnyuy.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gxdlrmieg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gjppchivy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfkyajfzd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gqutuwsqj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxldcwykb.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/giqucwlev.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gryopqqoc.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gsvrjqrbw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/ggoyrcyhr.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gluwapzfp.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gyaarqrvj.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gtiaacusw.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/ggoskszkj.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gblvxuxhc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gzewsumfz.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gguzwmxtk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gnznvoyxx.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gtacfvhdb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/glppoxams.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/glzxgdlmt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gpvyngkyd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/grsdyrxbc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gtzynybhp.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gcpvzkmaf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gynqhznml.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gesvbwddm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gcejlozdm.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gvtqcmoaa.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gwmrhufcg.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/grctruiom.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gxgnntzxm.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gvjselene.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gpqabtsih.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gmytmzoes.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/ggyfhkfuk.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gaiwdidor.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gkpbdilkn.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gmicxtprh.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/ggaumsndg.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gkuxvzlgv.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gvlecoopi.sHtML


<!-- 参考信息 -->