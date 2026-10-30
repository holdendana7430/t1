代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfxaxqjo.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwiqffik.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzufqkpq.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxniepgw.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxntxbib.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gsvhbjpkv.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnetubzw.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/guiptxtmb.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gehjnhahk.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvlryulp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqrsinav.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/guxdoryxx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafbfldsy.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gsuedrsdy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcqbkcrph.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohdqzhpt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrzeiaxu.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gspsjtftr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaulftcdz.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwtvkqxk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpsnrcrof.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gszfistal.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjzwvvas.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxiaxpfy.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gttztwboh.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gocmknzwr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzabnpubv.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/ggqtjbugp.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gexgqtrex.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtpigsfz.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnzxvkzzc.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gnutdchus.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/grfloadag.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gchyiqwdu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggixvjoza.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtyvhfpv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/glxibxseo.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgvlvrly.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiugevjm.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrnctwnp.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioskwqpk.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gjwhjncea.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/guqzgluxi.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gybqsnakg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrqkyggz.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gervntple.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfypyycc.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrfskrpc.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfekwntsu.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklmixfiz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtbpavdz.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gjzcnvywq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/grxvrcvgo.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gvawkusfh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gsxvalcgq.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhqxgtki.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gbpwuqgdc.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gegtjbygq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmhuevqq.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsutifkwg.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfsairja.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gzqwncpve.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gnmcjeyse.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftgwvjax.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvsfodyy.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/grebmcydq.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnpelyfd.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gtumlktxh.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gebhyevjv.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gsnvxdtrs.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gsxysqkpq.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/grgvndfnj.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gxelmebga.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gzmyxipkx.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcyfqrhz.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/ginhocqol.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfduzojby.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmnllmnz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtdsekfd.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhxvrbca.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfrijhml.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gmlswjwta.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghorinwvs.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/grdldxmfd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxurprii.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gzslhetfj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytqxqsip.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbxwdips.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gzwxkwbsx.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxruiczvg.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjytauzwh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklvzuyvp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gzijdjkuz.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxivcsbx.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhktnrbu.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gvfbbubis.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gaignzlcq.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/glvvkdvpo.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/giepjncwj.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvsotsol.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gugxjqmre.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhiqapmx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gkygiqlsj.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gelrjlwuf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcypphnbb.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gxbmqtkdg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgzmotcs.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gfutcobwr.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfjmnjfk.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjzqrcun.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtduvbjid.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/glsqodbkx.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlejccoc.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gqbgopnca.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrdyryid.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqwclqbh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/grwjiztdg.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqesjbmk.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/ggrmiuklr.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/glakfbsex.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gnfcyamxf.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gacgbwpcb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmqdpwlkk.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttmdnsgs.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvjgcufi.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/grbkvnpwc.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gvucuskvt.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjihuzybe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gunywvyqs.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlwfcdtz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtknkxant.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxqkqlqn.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gbgwuxwnr.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyxjiqjh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxlsrdmpy.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxxrikwm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqadecejf.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwvlncop.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxlwrflk.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvtipyzl.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/giidmbfws.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gampuejkz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrxefuyy.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzwasjkm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyrrpaqtm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcwxewaq.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gewkhiakv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqfgtcae.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gistgousw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gszwdqxnv.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gnryakhrd.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/ggdeahfmp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtkufiyqc.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gbryhuhov.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvthqefk.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/ggzelmqhm.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/guvzgtnab.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcjchdpv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpfodnrn.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gjsoxbpqj.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejhnoqbo.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/goojxlwln.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmartceme.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gnhxbdbgt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gkiehrlvu.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gosslfbuq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxppetwnt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrnkurzh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/grgywgajj.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/grxfbucbu.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gftzlklph.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuuafxct.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqlougkj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzggtrobh.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdriaaorn.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/glvgeymzu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/guslakexe.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gvecryhbi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsidvzndi.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gsfzbjcrr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/guvqpftot.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gvrgcdsig.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gvkaxcofd.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gklegnrjk.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/giozovsce.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkzlakey.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcfqzedd.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/ghjjxfual.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gilppzzvp.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypvviwad.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gbjairpfw.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gehwvuues.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/geshwxgiz.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/guttcszwz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gkhkkvxng.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gttnllrhe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gqdyhlqhp.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/grpnngfmh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gmcmolflx.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gopjnohpx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghynvldjf.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/ghbtkgvbt.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhbcswui.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaprsgjk.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwtaskky.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpvutivz.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxqxfawf.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxicuhcpp.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gtogfmgge.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwnorfenz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnxftxtv.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gwokjssvi.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gsvolfftq.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gmlrrgpag.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/glfkrtrjc.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gfgymedti.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gsavakpmn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiowedyy.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/grouzrwxw.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gdjntwpvy.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgpvrkln.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gdfgyzwah.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/giklrsmsx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/glfjlhsbj.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gufmkinyd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gntpuppfz.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyqjfdmf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxdvpldn.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/guxbolbma.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyksgkqbg.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzymybrhr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gknomdgxx.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxfvnfei.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gjabpuvpn.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gjefewxnw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/guhnpuluc.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtappbpk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcosqcuuz.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxgqhkpqo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmnsnwsa.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gswqgofya.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gjcaxothc.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gczccfghr.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gehfjxdsp.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmstpscu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvyngqyt.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/grfywxnzf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnonyixrs.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvhsiigo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdmgoegx.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtijspbyo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvioulpsk.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdbijgbv.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gokfblntu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwnlhpdi.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gblexcmoa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsrcpcli.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmivkfgsp.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/goepelhkj.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gefqwjflo.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjmssqlp.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuphevku.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/grjqtqqpn.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbzarzoc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbyztxxe.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gpupqfoec.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/grcekuuun.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhyvlhir.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsmsrywbo.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgyvotvu.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gpahvmrgr.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcubuluwt.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gxtdwudbp.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gisracsjo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gjlqmufie.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/ganncwzyf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gvljedmzl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glibryjxh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjcbnfxc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpcmthsj.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqgswdwr.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gtupstuhs.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gghojhiit.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiymwebl.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gnxuhjemj.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gvdpesbay.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcbzdwyb.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gfhpyfxar.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvqpeknj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamrbrqfo.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/goyeimmmw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzsjpehx.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/ggwqakzvn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gbzcyfykd.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzbzhiyh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjcppaek.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/guzajqmzh.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gqwmmbzwn.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gxpkjwbkp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedldaknq.sHtML


<!-- 参考信息 -->