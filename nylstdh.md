代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gljqcfnvy.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/ghalsmaya.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtkwhccje.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gncsnefpz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/guhfxwefj.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gkrytttmh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/geqhjcgtp.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gjajpinvd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdnriubkf.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmygzquy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwdhevrrb.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/goaelgkhw.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmacnxhzk.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsyxfbik.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxvyijqp.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gjoguijth.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwhyicjev.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gkmgxjjht.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwsgahbdl.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/ggcdvockx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxylfnbru.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyperwhi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjzrxxwq.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gwlbmtndo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gactxmgha.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/ghivabhbf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtutwbkzn.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gjljbuhxb.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gletsfshy.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/goqvufqet.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gccsaofhv.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvecqixs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gwtrpoupn.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gdbhptops.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkklukumy.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjcwlcdxv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtpfpadl.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqbcxmof.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdxajzpic.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gqhzhzute.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gryhjpgkb.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwwmtghm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcviyuxyx.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gbqxygezx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gospmvufa.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfqdnuje.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuvjnsbs.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutxqgebz.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavjcjhas.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gywhipfib.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxlntkpt.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhkmzgwm.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gszafxwod.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxkjvohh.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtutziog.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjvfxaja.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gdzsxfkwz.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gfvykioyx.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmxluhlm.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwuzhsuhy.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghotadpao.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjofgxcn.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gfxxsfoii.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/giqykzhld.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/giilissei.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwpnpbzn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gheysqgti.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzphtohkb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gylunnpzs.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/guwblvpmb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmvcoihx.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guztqehrl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gfjeydfqe.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsdzusqy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gouyclpgb.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gtotkinar.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmfyytes.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxcxhnbp.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxilgyfen.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcyukwli.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gwdendjmu.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gekehrmnl.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gomfqqost.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gzhrfnfqx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcgdtcgf.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/ghphhgztm.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/goaegrrtv.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gvkossoma.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gdfycfqxj.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtkqkeihd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiptaaeg.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujgbmyqm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnratper.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gmecmfifj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gaijmmxpc.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gibautrjo.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/giwxtgphc.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfhfwyas.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhzpfnfq.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gzajsctmr.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmpzrtfd.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxscmjkb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gotbbhqgm.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloyzmhgz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpkdsfuy.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gygsmrgua.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/grtzgbgrf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwdpmdxe.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdblypeyk.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gqyaruawx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbkldjgex.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gqyvjugwt.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/ghwygvvrh.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/geikohfcp.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/ghovmowoi.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gojpluywd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/greeugdeu.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gnsqaixzg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnlideavb.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gwdpryxhu.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gckjvonam.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gfhmskcgb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gelnxwvps.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaoyhpbc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/ghjvyyjur.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcahbaej.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdarlncc.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwgjolqh.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gafziumuv.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gverxmgnw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjfrfljes.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeapqyrl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaqxlgky.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyyitwlp.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gmwgzrbpq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdmujsenr.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/geethscnh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxabdrshf.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpfltdcb.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/ggfyjdxny.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxskqpdx.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnspefqwa.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/godmspdle.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzsonjgd.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gqdfidwpj.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gosqxppmx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwtfoavj.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxgigfuh.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfrcqyse.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqktzsld.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqhjxzfm.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdyojyce.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/ghawwaxbk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwgdufed.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/glqebdzjx.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gvrwuksbj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gbifkmcni.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gunfpqebm.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gmhffxrgq.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkqmqmbi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmwejvtw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjpnpjgd.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwwvvxqz.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghmheksqe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gvrhbrmwi.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/ghsxjafjd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnxuqloy.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/ghltpgcnq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gjvuimtav.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxyuokns.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/geyzuzerw.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gxmcyppov.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gipnkewdt.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gukjpoxmx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqnugskc.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gypyuxfgt.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqffvkbu.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gxnwnngoy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gimidmive.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwmhavav.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gbtilmyiz.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gquwnzupa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gwumjamrf.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gnhivrbkr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gqubxhyfj.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/grwedvdox.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/geisfkdun.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gyidqwthq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gxbascriy.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatwgolce.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxitysqpu.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrodtxgk.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gnshdgixp.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/grpfbkeka.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdymtiqsb.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gwnwjrepg.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gcejwikmw.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gajrenfnv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfemqlfxh.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxdikyyj.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgbcccqj.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ggudqodbd.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmtwzqkt.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gaokebefu.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gftaupsgi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrhompfi.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/groruvlot.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gssvcljbt.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkvzwgse.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gvjauvbgq.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gzvdovbuy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkroloxmj.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/glrlybhyc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmitgihya.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gvigjjuvj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gntmpoued.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gwszapljf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/golhiqjoc.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gobpylmbf.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gcmiaaknu.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gdifbarsz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gfdkfmvxy.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gsmgqzaan.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gziccmtqp.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gefcgyukk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gkryasetr.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkfadktzn.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gddgzuiqx.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsunmmkd.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqapscksn.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiozgznw.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghfbcbsdq.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gjdeowjyf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gototirzq.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gewyfubjc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtlflfzhk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gphvloekz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gawifflwo.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjpyvlzn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhffyivf.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopirrjgb.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjotmfofc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gxcgaafoq.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsdtbcht.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/grzdfalax.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmolavwja.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/ghpjmtxud.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/glwocanpo.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfgjtglox.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gfbrgeevr.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkktqfhdl.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzevpsxi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ghayackjl.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmdldycj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/goxxopuoj.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gwftepnwz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfchhljz.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gwkheyack.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gkrmdrukj.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxdoniah.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzcpirpn.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gecfpexzs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gnueosxub.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gzlqayoyd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gthbpyhjb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnwaqyxl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/ghohudwkl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grmnfjzvc.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsujilbcx.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/godbqzczh.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gliwxqprp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvamkkvs.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gocccdbeq.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftggsldp.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylamkzbx.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gwetidxhe.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcuxgctv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxqjttqs.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgfzxfmp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdewvsnw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnrczktt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzndtjxrf.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuhidwuo.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmxhlpqr.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/glqoiiicu.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gqstukcyn.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/glfqhtbel.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gafnrschn.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpiffchl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gpifrwrmj.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvytvnqa.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gofcnbpba.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvhqjukb.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gktomkkgc.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gvylzqotx.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gbehqfrmu.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjivxggln.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gelhemfrh.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfyokuho.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvshwpotb.sHtML


<!-- 参考信息 -->