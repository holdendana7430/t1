代发 wailian999

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkuaxzmq.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfkavsim.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gukahhotm.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhjtmkfj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlrnzrpj.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gofohkqta.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogpwzpjy.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphjxxsra.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufkzrrcx.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvspmsuvt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpdjxdqzr.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graomwnes.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxdahugi.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gymuqbnmz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzkcrhcdx.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsjfgwqg.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gacwbbzrb.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/glyzrkuvp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gypalnzin.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmbbgfpd.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdlsrpemg.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmhzvhmd.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevmnxhng.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gdmlrwyup.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gujbvniwn.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/goookxdgn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gktbezbay.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtzsbdny.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxngwzfq.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnijyfqwg.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdenmjgkg.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/ghabzjnan.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gtsxzvktj.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gizdnszer.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndrwdtyf.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggihpgida.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gplewkeln.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluihhwvw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/geyhxmiwq.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvvejhwg.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gitunyszi.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/guturppxa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/glglravyq.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gqmidttcf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdyqikvn.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcrrwuqx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/glyztvxqe.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gvlcxfryn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoztnbfi.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqtyvocx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gijajrzzz.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/ghqiuzhwq.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gzdzpxork.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gdnbmjpid.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gaefqbglv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnkrzczt.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczrbpupj.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuufuiit.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gpynsdzvu.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gkpvekcft.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzrzrsyk.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/guszzlveh.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmmloapa.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwxnkzxj.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gvofvkosa.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrfcftha.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gmephnnfg.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/ggwmimybb.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/ghpjeweej.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gpggoojet.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gulijldgx.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlwntkow.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gpzqcdmen.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gqexhvnzt.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqgjfcnf.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrdumiis.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gnxaywrce.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxkvophf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsempdgc.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbenrzzn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjryftcb.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwybsyph.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzjxiknef.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcbsvlnr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuusioar.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsevtmwjf.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknoxljgx.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gzijiqhuz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdbwdqds.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gvmhvqmni.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzbjrzdk.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviobzeen.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbvwncij.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeetozwm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gnhtsvrjg.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gkdwkwnji.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gdlggarqh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipxrqwmv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmclxojyn.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbdajdwy.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnozwgep.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsciskdsy.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbszrkfc.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvboqita.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbkpdcay.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gojbfedse.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdozflhv.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/goaxgbosw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpqkglyv.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsqhjtvi.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrgogahq.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/giaeyzxrh.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpngfdnd.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gvpsijgda.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnunysqkt.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpajzqtg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/grvuoeuqa.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gadpkbght.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/glxapeqzx.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gxqscvups.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gotyycfgi.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gnkzlafps.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gsaecnlfj.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsuhvuzy.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxaavsdd.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gyfjnclkc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtvnbcwun.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gztqipcsh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gcxwpudhm.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gebyabkte.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/godzihbtp.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzbnhrtp.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gwovpvmov.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gcgtmwgkk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkkvenva.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/goymckvkg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvporyplb.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gohvfmzuh.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkcgesxy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbkxaegzw.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gldyrkfng.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkmwmxgy.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgztzivj.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gokrrbqkg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gshylxepo.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gfrexjxja.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmeaapxa.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqxofkjw.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gescamngy.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gfznybdso.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzepwgkgo.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsagbeypf.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gkhpuojlh.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gxqnqpizs.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkoavwlf.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbohfmpii.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gukrbmnzt.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gfqsfssrq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqlzhdjb.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gjeqebdxa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gagygcggo.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gpujuemsq.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlvspecb.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfhezgmvw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genptevmn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqddbhjf.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gkyrswrwb.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsjlkbte.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccswxmxa.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gxekpdhbb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzptpnpus.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gkjgjehzg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/ggakxbvhs.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giouidlbc.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/glgatgesk.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqmauywv.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gbluxkomi.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gmogatqtk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/glzpbxvql.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqikaawnk.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gwlxhmfed.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gqtuqztsf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdbdnvet.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvpzbaxo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/grdmhalhy.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoeyeogu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gkleirpwn.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gkjlrgekn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/glvqndnea.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkelmchfy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gylolxdks.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/giqzabrko.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/ggwihzkbs.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeatocer.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gdvzummiw.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gmupqpovg.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/glljencpx.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxfvykqg.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbbpmdlb.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmbiarkur.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/ganfzoila.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gltjsxqsp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gtblgakfu.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/grirynups.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/glntxzzlf.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gtiabvfaf.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggddemhud.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gormpctob.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotfgouqt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gruyefvvh.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gansoroug.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzjkswty.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gmnzibwvb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gdidbzkbq.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gzahxihxo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpgruqtbk.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduuraicf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwazvivf.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gzpyzccez.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gagyrhuyh.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gpbczfpsq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjjrvcrp.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcwsipgk.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gixavxhwj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasyvdacs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkwitbel.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/guempnwpy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmefcfbn.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzobqcqps.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gmccivpmf.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gulktjgpt.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gkebthlnu.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyctijlj.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/ggflnfqtj.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvqrkhja.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogytexih.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvihwcxf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/glsbnrung.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gbaasbull.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdkwbxtj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjelpprf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnpysrfdu.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfqqjofu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzhaydnf.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gttcykrrl.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/glqpzqxec.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciuxqtxu.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvsnraru.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwwedgcd.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwesuvoh.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/geitclfak.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gjhhmabns.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxvemeumw.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gytnyqpqw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcfgisis.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gfknqschk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gviqphkci.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godgapozr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkwuphhm.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gtznlevsm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/guyljedqz.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbhehnct.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqukklhak.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkaaiczz.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gimsfjldx.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gdgmtqiyd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gukesmbup.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gbojwldlz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupfllhlz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfomshve.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwczbalvp.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gedcljvuq.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcejsbrs.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlmgofsf.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gojgvdipa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnmxtosy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilvyzzum.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzjwghau.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcflmiylz.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gesyjbhre.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gocoqqpva.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gakupjzbd.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/glvynthvu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gonnblntw.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gwqppfvlp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/geqyrifvx.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgabfjlr.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gmmhxykoo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpevqewd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/givxwxrvp.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gmvoisnwl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpmvriql.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqjqemze.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/grewppovd.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gbtkocoyg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdwwmhge.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbrzvavw.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gtuhpdabs.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmvntkca.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gaprfutth.sHtML


<!-- 参考信息 -->