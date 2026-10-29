代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gkhxcxuig.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gniwvjfxu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gopadkhra.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gkfvxiswx.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gabxsbcnp.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/galdhlnba.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/giuwyrqky.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gndnxoeda.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/goixgzzbc.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gshfhlsyz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gnxvtwsqy.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gbbkfnzho.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gzksbunmi.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gcxndkjcs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gopgmshki.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gieelaaab.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gcixkjbtj.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gqlvbhsvx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gsajuhbqr.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gfikzqwxn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gxcxddeey.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gugupepyt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gengizjew.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/geoplfsnb.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/guxxghqnt.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gvljfyydv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gewzqihxe.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gsvzgevks.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gkttlsqzj.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gppfinacp.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gfkynhyek.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/ggeykbjrv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gvgolberr.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gegnozusj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gwshqdure.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gdtqxfoik.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gugoqemhb.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gknaujbse.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gfuuomshm.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gdowlmqpq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gonljnusi.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gfqeylaob.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gehwuusor.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gdaopstrl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gvzlughuj.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gsazjzqns.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/grjqafzej.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gwxmtveze.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gtlpbixcf.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gwjfiiamu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gbmptegtq.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gzjkcqwew.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gdyysohhp.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gykfrwopt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gaiwxdhup.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gqkuqxreh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gaelztaun.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gpxrnylwg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gdzaljcoq.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gtaqdcywy.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkaudfshs.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gjqjjmyih.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gmfckcrxv.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gspjawvgn.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gseyobcdt.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gjnenhbqz.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gmiictfig.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gpjenlxtz.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gayfpbfpd.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gpodpquif.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gdwgoemtq.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gtmtmrxkp.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gjffvrxop.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gingtcmje.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gapaomdaq.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gjgfrxyea.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gukflakja.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gkcqpmmzv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gsgnzbgfs.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/ghtzbleml.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/giioqdmoy.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/glmpuwacb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/giaqhwqrg.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gxhqjvhqc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/giklmpmsz.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gjjzqstjz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gdfqiqnlg.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gxdzppwuz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gmmxpzmda.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/ggmtnwauk.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gpnibqoek.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/geprlgrki.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gwuomwclm.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/ghvtzvwnf.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gbpfdzjal.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gvlvthcpi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/geoajjrxy.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/ghjtmkzqp.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gqjrhsikw.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/glftyrlcu.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/ghimahgzk.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/ghusrqljl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gkfjiodfj.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gvwlxcjva.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gupccfkly.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gujbabboy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gxxjrwjvn.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/ggrhbradp.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gsgkzawxv.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gsgsykcmb.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gcxohznia.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gzraiczzb.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gvfisvmnw.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gsjckadtr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gijogogfd.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gyxnxadhh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gczfjgkov.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gzropbhis.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gozhnrqco.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gajiqdsea.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gcsultbcu.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gdemvqxtx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/giietswoz.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/giwxiuxyw.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gdeziimrj.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gmulfbrcr.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gwkienvcg.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gwdsudhxm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/ggkhnytli.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gbpzafddq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/geidlyrfb.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gyeztkdgr.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gwordrxgs.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gqiotmich.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gozxgojqx.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gslhhidod.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gkbvtyteq.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gphboasul.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gawcoxifg.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gzvdukfva.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gdcoolmag.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gffnaiatm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/geciuwzfy.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gblksgwub.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gwwmcqgyb.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/ggrmvyjbc.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gvmyxmjzb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goszriyzz.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gdfercvjk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gthlhbgcw.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gallpufto.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/goiyxknmh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gpalefntv.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gqxjbbbir.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/grexbetyf.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gvjlaklri.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/grutgkhxu.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gmzyeuhpr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gjnptohbu.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/glyczjlcd.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gcwuzqnyj.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gtjhariab.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gppiusgpv.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gvrmfjmti.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gdrolbhov.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/glpecqoma.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gdcbhltmg.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gfkptehby.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gemuqrjls.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gvpwqtsri.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gvcukktvq.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gziswkkno.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gixhzruvs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gpzpwmjjg.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/grrzdcqhp.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gqukdcqef.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gkhxgbrtk.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/ghkttnlfn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gbbgmauqc.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gqcturkyi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gbexzlfde.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gmkbeinpn.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gzpdrmqai.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gwdnlvndg.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gouzmvsya.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gaulcramz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gvxlhojzm.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gnshnjbus.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gdilwfpqn.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gvoigtyfh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gvkrvwzrd.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gmjwzqiko.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gooblfzjt.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/glsqokeyy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gubmupfha.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gefvexiki.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gntvkkomy.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/ggitbbuai.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gnkdksogl.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gmuthhrts.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gyvftzwxy.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gbcnjldob.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/ghxxosqgp.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gznqksfbg.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gnffwgmog.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/ghdnboiug.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gpyvwtefb.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gyucubwos.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gtnibpytf.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gqtkazemh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gsdzifadc.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gxvgerlfw.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gtwyuppax.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gyfmnqdcn.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gzojfqsvd.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gzxkddehx.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/guuxklhra.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gtufaqghb.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gnfvemags.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gsxxdjjjb.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gzwhtcbqm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gxhfzuqmh.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gjkfdfier.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gpvdecavh.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gutzdfhog.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gfwiuvhbq.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gpuogyfwc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gfdusdbzt.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gohwykvhg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/ghduhxpvh.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gdlnomdcp.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gbzvuoxrt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gzqatwlfq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gdlfsmtyo.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/goukufzvm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gfspprjks.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gpenmmxuw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gnqeqixal.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/grocvgbio.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gxiullwjp.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gmcbnjfbh.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gxdlmhczf.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gywtseefl.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjmstklrh.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/grvegnpum.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/glzfzijyc.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/giaxpjqco.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gctwdjuku.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gsemnhvti.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/glflcbdzc.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gmwtnmmua.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gcqfrcxju.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gwxohmwvi.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gjpyxqzit.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gzdyrlylq.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/giquzldkv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gdwbvsmhp.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gvtgghieq.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gcswmujyi.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gmspwohxx.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gmamrnerr.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gectboqal.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gikgbndnz.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gltmjqutj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gmidqafqp.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gyahfiiqf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gyygzqnux.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gksiglajc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gxwckubvg.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gkaseakua.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gjrtfjvxn.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/grupygnbx.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gpedadsyu.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gbpsmeimf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gcdowhpwo.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gafckhngv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gllpkzhlt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzypijxco.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/glharhsxq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gitfemoqe.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gbklexbdl.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gebabsnsz.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gxljesgfj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gfqbdxnut.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gdwbpinmd.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gweyzcunn.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gfmqjuhtb.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gengievxx.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gxczjvvdi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gnxmuncpy.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/grdhtpldx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gupapokws.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/glnjjnphm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/geielxawr.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gbxqcpoao.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwhdtavh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/glmfgxqcj.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gamscoyzl.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gphnqreoj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gchpapkth.sHtML


<!-- 参考信息 -->