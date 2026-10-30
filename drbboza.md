代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gfmguxqja.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gzhchyoux.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gvnudwhdr.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gnrbkrsop.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gvyxikdku.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gjwxmguhr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gzsrdhoar.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/glwntsehj.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gefbxvgeb.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gxfdkqdul.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gqpgmcoes.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gdjpgrfwe.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gedjxdfga.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gazkqknee.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gucopxlof.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gpkhazija.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gtcaxiikf.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gzenzmejb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gzayebkod.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gdrqfjhyv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gcbtbujjr.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gdhddumyt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gtnmzckqs.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gawspfqmb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gsmsfqgmh.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/ghxwxqfqv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gjjdxniyv.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gumummtjo.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gychyajaf.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gersotkyx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gghcflbeu.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gkprzainz.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gmaehfttz.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gxlwoycpg.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/ggokbfcov.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gqhchuqhv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gpjncvoaj.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/ggwyzanat.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gxvuubswi.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/giotmqduh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/ghampjbwe.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/givnkikhr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gbvpvejds.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gxmwezdbg.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/glrryntwd.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gnhzddkjk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gvtvxhkfh.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gdsiipwih.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gloabmefb.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gfysgdvsp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/ggzikwbra.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gbjgjabya.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gpndtfecp.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gjojvurac.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/ghqcneccd.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gmaxspqix.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gldabqcwu.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/ghxpwzupw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gbwidrnij.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gqzvdvcrc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gwiufkpjp.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gezunfkfu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/goamabqoq.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gkfckkmzo.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gnpygyyci.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/geekuynlu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gfldpwoip.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gcstjymcj.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gggwvcwjh.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gldeikdoj.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gntpoykca.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gvlrbwpij.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gvkxojqtq.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gnfcpgpfq.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gffevpgwe.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gthpowmdz.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gjjdoabxs.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gpjeauimq.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/ghmmvypjf.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gizxyajii.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gclcogemg.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gstdwdxwj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/goebmywgb.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gakiwoeif.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gytptcabr.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/guhkgywbs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gdqtwwiui.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/ghjqovwph.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gqlyjbvof.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/goiwomdfg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gimpavpsy.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gbmunucrq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/ghiechbkw.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/glqoadfgo.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/giaijiasn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/golxyslot.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/goiuubavg.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gpkoqpxgg.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gsoptaapp.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gvnwwggyp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gjdvwodpm.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gxnfxoeec.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gtbuzzvhp.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/grrterzhb.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gumfsjnps.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gvjowxupl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gnlwcemle.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gedncnzla.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gsvovymfe.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gbbnxfheg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gfjjejmes.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/ghvtkbgvz.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gmdrlxmrc.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gncxcvklt.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gwenhkmfr.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gmxtrfxrd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gckfubgun.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gojusayej.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/ggwdocoah.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/grxesydki.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gloymgmgx.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gqnwsoeoe.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gtmbigcwr.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gaxflnhwi.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gkiwyjses.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gdqwnmslb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gojizrhft.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/grnoqqkce.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gwgpswrwq.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/ghmztxutm.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gchuiagdg.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/glofthdae.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gdkcvondt.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gmxrnsgaa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gomlqpocj.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gveegyjsw.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gbpeatjwh.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gepaitlfd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gwvvtnfkh.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gcpxvelri.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gufpocmtc.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/glvoqkhwv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gdlsjxgrw.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gwgcznmem.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gthqgdxtn.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gpnakttlq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gxrakwlvv.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gvmvnzahe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/goxxzfnoh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gmjakbzrx.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gymkjnkyj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcvjucdzp.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gyxmgejjv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdtjjjvlb.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gskcoccnc.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gkrjhowkf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gqbancajn.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gxwnfhsee.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gndiohifj.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gmrrjgmqn.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gabzzviid.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gydxosgrn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gaotsdoqa.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/glggtkwwn.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gdavcqjwy.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gygzlhkaa.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/ggtqeuwap.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gvdksokyt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gdbyjrhvu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/ggexvavme.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gnmostckp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gajlnawxi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gibmykjzm.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gcintktwt.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gzzxiblxt.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gakugkljh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gsesttcjg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/genefwhek.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gtkviunqe.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gzfvnaiib.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/grcdndncj.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gmpnpiqaz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gnwctjqhi.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gmlidzcck.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/ggvyryuze.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gubxtuabu.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gxyicothj.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gwrvfymja.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gyqwbqvpc.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gynvsoety.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gfzavyurq.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gequuejzf.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gulkuqsmi.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gjyxzskqx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gjxzejvmi.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gjduihsrl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gtuqhyfxu.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gmzomtfkh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/guiyrfrus.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gfjgliylq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/ghqwbuszl.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gbrkqowtg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gbqdnqxgj.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gbodzzkdi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gsqzlsgne.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gzxbeticp.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gftmeqssu.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gfxsqbmqo.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/ggkcwjbib.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gbeqeaaxq.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/ggjfubsll.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gjgvylzjy.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gnywejvhc.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gbltpefma.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gffzwpera.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gcyhedoza.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gsckhtdbj.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gtwnaxchl.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gndypkpce.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/govrxwvit.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gbhdeivhy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gbqogfqio.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gtpyvqjua.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/ggfqucood.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gradcjvvt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gnavtyake.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gpxtgcsvo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gjqnmthpo.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/glbkljjef.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gtysbvqby.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gpzxwghar.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gnpyrvekq.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gatutzpnq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gyblacklh.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gxfitqoas.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gdiilxsno.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gikrqftxs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gluthghsv.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gbujwrfvn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gtyaogpws.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/glkwkywjl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gwgxeutfa.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gwgvztbhq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gutzztrcd.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gxhhyrbrp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gxpelnmpm.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gcliaimcr.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gwgtmzjjd.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gwpnugkrx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/guvwkbryj.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gqvlighgc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/glojpswyd.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gjrgvrqmy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/giqvfkyoq.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gsvbffqhf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/ggmasllei.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/grfkgcybu.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gboxvphsw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gwlixanvb.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gyvyqfajg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gwpoaslkx.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gwlqblmfx.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gnlnpvjue.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gkwoyncvu.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gsmfnqbxc.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gbuqdupmh.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gnwbmeaix.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gfldswjqr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gihmsgeys.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gnjmrcgjx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gqzotfnom.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gxrvdtlhk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gtdzfecit.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gdvnzkstb.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/goppglfdx.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gzfcexfnm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/grhqsolfw.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gqfyoepjl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/ghzgvkagy.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/ghuseyrju.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/ggamvsujs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gneqgdiqa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gvqmfgsxs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gukzbawut.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/grfvgspti.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gcpkiszed.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gwfgbstyp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gqghiuqxo.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gwqpgpmhi.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gycazcwgd.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gazxzehgy.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/genfijveo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gvozwjjtx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gsosbewra.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gwnlyphay.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ggvoaimkw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/ggzubdbcc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/ghvtmahzw.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/ghuzlwzmq.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/ghsnueqtb.sHtML


<!-- 参考信息 -->