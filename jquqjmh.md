代发 wailian999

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gfotioinp.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogfildyg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gipcmwynw.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gfeowkbrg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvdmtylj.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gaioesvhw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqqyzxsw.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gysfdzdif.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcyzwgkhp.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gomhgybiu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gegooamdr.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzhaldve.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqnznfql.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gpatukbhu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ggvhuqnoh.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/giiokbzkw.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopjgixqn.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gissqitwf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpjstomzo.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gjnouryfh.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvmzkydgf.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gbtourqiq.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtbkxxioi.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaufposm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gppblrhck.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gltnsgbgm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlmjbshw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxeroqtr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwivnwaox.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gzaswjmei.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gxucapdjg.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssozapgo.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gispvyydk.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/guiawixhe.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gibxsdkzx.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfdoxbkox.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbjfdajr.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gdbnbusmv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gllndhits.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/goupzvgic.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghibkjyve.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzslcjoi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzrasvbaa.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gubofpbxt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gukflqhrt.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gexghypip.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfepcjka.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnjteoon.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaddsjldp.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gosjnhcll.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gpyzomvkr.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gaitorhda.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzsforue.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/grqgrqtat.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxnnbyzv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gegpewhar.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfaqmluz.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvablwqfz.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/geihukjzo.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gpwiystsf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/giowxgowg.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/grogvjwik.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gppvhvdwh.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlegmwev.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gdhkczugs.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganfzhobp.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gkdhlzmpo.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gujjpugcz.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqrpamvy.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxtvwlhm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhdxbuht.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxccdxiz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuhqffpw.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlxyfulq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopnwvdtw.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gaywvaelj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnpkwlal.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqbayadi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnppigdf.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gatmjpwii.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrjbmros.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/goykmcxnz.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfitoftd.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbkjrrtd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gypqxsibf.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjifbotjd.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgdsymme.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gvywrhmsv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gnxvuppvv.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gbvvujpjt.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslzbyyjf.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gssuttneo.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpygspjjx.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/grrrmmscu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapbrqmbd.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gipdcqpcn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtbzoomn.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gqezghbsg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqczeild.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgfinjkw.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gdroniqvu.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdjvuvnpq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/guzzlykux.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgnprtcb.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/geiqhqdlg.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszcaaavu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqukpzbb.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeoilxwm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gcsfaijoi.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gzmbkzdeb.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/giizhaeum.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrgqsfns.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhvcmikp.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gpfzzvkzi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gazqyvpmu.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gplieperd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/goztlxvcx.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gurduvcrb.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvituaen.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyvqjthk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gxrlysrcb.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gugxngxze.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goylrmtyr.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gvzqguumm.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsilgnui.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gfsegnzrq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkdkrply.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymagepmm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/ginvhlwoe.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcvupuzvq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gcfbczdex.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdmqpljj.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gonvzkzaw.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gftkhaxio.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giepjgdwn.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/glkphmthv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdvfxtnmu.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gzmktbfrc.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxnpwusv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbheyjeii.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmddexpmb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/geafolufo.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/goacxhotv.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gyqwrcxtn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnemrwcsw.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/glcrhgica.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/ggzjqiwyl.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gyovkyqrk.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gwcztycub.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gpgwuqabh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjoewpdc.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gasgihokx.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gfqdzlqko.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtqkqrru.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/ggkbkbvfu.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkretywl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gtcxgujrh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosofcuzw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gurcumxwj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrjmbexg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjxhgguk.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfhgnjtk.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuqjjhhi.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/grvkbodmr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gxhakialg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhovvrjq.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzybipjd.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypprqtgs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzpzgckc.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gcubjikgl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gwpaettwn.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcilybzc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gajtxyrde.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gtdhthwkh.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxynwcto.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhzrnhjj.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gfpewvifs.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnumsolh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gcxxdefnh.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxfgbehho.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gktxhwuaz.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxsmjkht.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwxdklpf.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/glhozalwb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gnhwgmesi.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gbabxfvxb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/grdkagwdw.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gozweibaf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/glbfvnrrt.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/ginqqgrcb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/geaoiopos.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gemfkuglb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gidkuswfx.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gunkxasmd.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gscdtbsnl.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorkxgpcc.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/guvxnzjgr.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gacvowupc.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnecfeejs.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsozqzvxv.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyejuigae.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gujjmrndi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjynzlnwp.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvofuqcjt.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ghseilzuh.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/goynqiqrz.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gomcjsdwh.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmeibapn.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/glxhejeks.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhsgcihe.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gsyzbjjsu.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/glttnfglp.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gldzslqgd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gyarzptng.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gckslhrww.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqemjyjzj.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gnbhtidng.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gssmpvwgh.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjmvvcrv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gfwieslff.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gqahaaqxu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowredhug.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceghiqeo.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtvizfwg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyrnqdok.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gytypbzxo.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxckvumz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gvzzieatn.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxeuqpdlw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjiikqov.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gahdsvctg.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gmrpolphn.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gpqfvdvfv.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/guqqthfkt.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiaeaxmu.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnckmcqh.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gqlbjtqkc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoijrjik.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdpaauhu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giacnamho.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmxmgaqp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhemztik.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxhoqbcr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgcodukt.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gndhaotcm.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcqnkwzac.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gcfpaxsuq.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gjgwofbrw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/glbuqgbfn.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gwnupyzbl.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gyhuwfqwr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gptizjshn.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guuhjypbb.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvvmnjic.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzswxhkv.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gthwtlztg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gijaklufw.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gkpkhztyw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goznzvovx.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gvujuihpo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzglqscy.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/grocbyajj.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqpravvq.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gvownitxq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmmxuvxr.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvbyyvch.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsvbdmbo.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/getzczbzb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gefopwiee.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grczvajxc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gdppvregv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gelaikpkc.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnzdkavy.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gzibfnghk.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjlevgfrk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfegimnm.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gmuvwoakj.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlxvguvq.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gkxzfdsml.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gvejfynua.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbprlfmxa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gcchddcsk.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gkqmmxelx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gngdabhth.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiusisno.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gghdzniai.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gsbejcibx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrczouhc.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjemcrkk.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/golcrgkbx.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gftelzzkl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdzxtntg.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gijdvehsh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkcazleh.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnbwmptm.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtqfumft.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwzgznue.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvivzybnh.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndqcqdlr.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gfcecuoxj.sHtML


<!-- 参考信息 -->