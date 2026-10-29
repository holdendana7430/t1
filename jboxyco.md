代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/getveydta.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gzmuozryr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gqrugwgiz.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gppgmgcpr.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/ggaeoymvd.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gbkevyyrx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gfornpnbx.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/ggeajyhzs.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gkvjxradf.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/grxrdzxxm.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gjoifkfkt.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gayocemtq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gwzklvqij.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gxhskmlsp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gbuarwhbg.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gtgbboivw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gykxxstcv.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gkruinxmu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/geuxlyjsk.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gqjgyenkf.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gcnvwxncx.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gyndnsnxo.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gesddqyrj.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gcyirqfbq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gijwxxunt.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gsemapeit.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gkklqifny.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gmzoayzeb.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gvciwoxdd.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gqokulvlm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gnpwfwpuc.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gabgkuuge.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gsfjvdarg.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gxpjwudam.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gdgtxjbbi.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gvjdbkkyp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gurjeelaz.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gskckwbpq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/geplqskoz.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gipoxpiun.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gihhtjbmz.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/glsiyohjx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gbvhmkccu.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gurjfittu.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gzbavpnay.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gxulnpalv.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gyntifeum.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/giqifwnpv.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gwesfjkes.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gabcfmuvy.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gqpwaubjf.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gcxrunztn.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gajodtngr.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/guaovropd.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/ggmksowvk.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gwdangzor.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/guzhzjeuj.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gaglldydg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gnzytvvtl.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gdwatfmuj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gzjxqzxiz.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/giifairhx.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gxkbbsiut.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gkvzhppcv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/geegitwej.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/guzkmaeem.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gnzqgulvd.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gjzgplgqz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/giigvtard.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/goktdqgsn.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/goatzcobm.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gibqcavtw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gwuvaxtak.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gevezhxgb.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gwzgryzxq.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/ghgmmbmkl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gzpfmzbfp.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gyvsximga.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gkdgdobbk.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gzatjhfym.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gqrguqzto.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gsinbadvp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/ghlmrznql.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gjecnajmb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gobvsuvwy.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gqrfeqoke.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gymskhsiw.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gihhgjarj.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gbxhiexbl.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gzoclgnto.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gmamcjjfn.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gnosdbabr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gqzywqagn.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gvrwdlfsa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/glqllqili.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gvltwpxfp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gxnlqqwft.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gylyhrcbd.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gvvaxnnwk.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gkpcqpluv.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gcsfjmwyn.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gfngddbqy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gzqfafrfm.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gtcjghvqb.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/glxoftymx.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gnmzfkkcd.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gyonygbgo.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/grcwxypuv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gfpjhovjn.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gicjhtool.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gcdtzcssf.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gneftwydu.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gjcledwqx.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gntiograq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gcmyangti.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmejupswr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gireulmgw.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gjngyvfll.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/geluttnlx.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/glkjgdemy.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/ggwdpnfja.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gwcqaznpd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gggefhbhw.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gjuwguztr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gjolyksnr.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gvypcswip.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gbaxcuarn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqoxcbdtd.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gdxsiezxx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghmqaslmt.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gtjznnlin.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gzcrpjdkv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/guucxhenu.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gkkaonjbw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gltzmchel.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gashvubbv.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gexerpgsy.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gxygwkbyd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gextrnpul.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gsubjcigo.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gjulwgjhw.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gmozxvrme.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/ggzdcxsmo.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gbxqlewkw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gilclcvye.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gwvosqivq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gogmcoyyn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gnjbkpvqc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gxcyzfhsk.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gpmrprfxe.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gaenpmjgc.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gmjjqvsvd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gvkxrwnnw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gzmztbbdn.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gbchwjqld.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gnaaqatph.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gfsjqbpiu.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gysxeifvd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gviemtulq.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gilszgxoq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gprgrtuuj.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gsijvpanl.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gnyktzcxw.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/ggoeusrzn.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/grecxsrzb.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gdtercdpn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/giwqmpmzo.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxolxxgid.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gsqkdqave.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gaxbwcppu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gmstfwxno.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gxtptkbkb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gnxwsufwp.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gpaveidvr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gfcrjvswr.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gnpqdrprk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/guybusjmo.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gtdjdskpl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gcxtlexyf.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gbflhtwyu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/ghykmrejd.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gihqzfdbh.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/grourneex.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gookoqdpf.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gwexyygkh.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gskshhzkz.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/glkeophmq.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/ghmozuhxz.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gsmdsuyuf.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gusweaxgw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/guofxyavk.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/goglezlxf.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gkgepbwww.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gltulhrzc.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/glxhpolic.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gsswyjjfy.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gtibiatou.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gyaeczurb.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gwhjgrzyb.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/geqcclwwg.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gtmzximnl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/geiqapotl.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gjfmhsraj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gkxsrlwos.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gdmxbwslp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gvswljhwb.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gjoskjhlx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gcnhjneax.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gdqipkkro.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gkyaresmi.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gjlttpqaq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gkordaokq.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/ggbmrpnuu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/grtgmvsqr.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/goiugbmgd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gkgewwxks.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gfzmicgki.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gocsakhna.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gkzdidbfn.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gshxepcey.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gwfvzioge.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gzrnqqjoq.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/galqgqcoj.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gtejrrpgj.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gistfybdm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/ghrbsddmm.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gcqpunxsp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gopiszntu.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gmuirugvt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gcfzyjmya.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gkbaplatk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gdabsckaf.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gnsdlabki.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gmptrkgxd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/ghefklhdw.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gkvyleksy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gtegmbjaf.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/glbekksjh.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gqkmptiho.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/grqjhntpn.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gygfeszss.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gfidhvpgd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gituqifqy.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gqmjxenbn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gbdsggiks.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gsrtojdbv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gbafwwrpn.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gcenubjuw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gceoknmrh.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gsocbmtny.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gkisqwlau.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gqzmekasu.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gcrawzyti.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gooiydmjk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gfyvwgkcb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gbpzmibqu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gtqhncfzv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzyoqcbdq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/glcezukup.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grtivhuyd.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gsmqxxsse.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gfkkziwtx.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gxzggmnnf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gmyqvkmnv.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gcufgnupd.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gxjhawoem.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gepbewaek.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gqhvsolke.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gopwzeoqz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gakvmcrmd.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gzchqgdax.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gjxpgjocd.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gqoauotht.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gvglqfafo.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/glmjctojo.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gdgyhagkj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gqdnrbeob.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gudfhtift.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gkuvyrqqf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gbzgzwywh.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gogcoaoli.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gcjaypgpd.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gpwabedpm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gsichfwzs.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gutlqkugt.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gypmakpuj.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gngbrrudx.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gqxbywvje.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gztmczngt.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gocevsbil.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gzcbfjyng.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gjhftwlio.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gtnyqcbew.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gkkgrxffk.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gtlptlgmc.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gllkwylck.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gkukztpwn.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gyfadvkio.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gbosqobnu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gyhhhqqsz.sHtML


<!-- 参考信息 -->