代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gliyrldrv.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedaljvgo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkxqdqbi.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkejwjav.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gnwifqird.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gwyewjjll.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqzofzes.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gvcrefppm.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/glqxuzdre.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gyahtfvnn.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/govivnyrx.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqjlyemg.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtydcdui.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzgzebzd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkhkzyrza.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/giobqysta.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzrzzcsu.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnchuqhv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gspuzjtcq.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcsaxgjgq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gupnubrcz.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcqfprog.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gyairqgiu.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/grlfdenfg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeggkgry.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gralcpzve.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqckzyhaa.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnkbynbx.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqlqcusmo.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/ggwmhthgp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyihscdp.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/giyqnzbyp.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsspmwtt.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/grfuolcsi.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/glssuthwd.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gtcjyigse.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gtjioigue.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcwhbctg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtiuvkwwr.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gtiqbqgnw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggqkhifag.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/guahcmfgx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsgcigep.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gkthimmzl.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gralxhkdq.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gcamgbsyj.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gbnsbdmdd.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggehyywxg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gbxqdtewr.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcnynroa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/guxjvzlnc.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciyftrep.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbpdqjsxp.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/glhwdyjzz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gabkvgbto.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqynwtlfc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/ghmiodyad.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxchxuem.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfipmfqqi.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwwasslb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gzaqnvzue.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gkasemgqk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghebgtwbl.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvgumqwwo.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grcrbceku.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzrxbxod.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgyxnosi.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/grtpnuvse.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gdbbpawbb.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnhveerj.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gpyfbeewi.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloubcseh.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glinymuzk.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/goflgighw.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtnbhtubp.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaepzdek.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gkpdfopqq.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gospqmbhr.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gonepavap.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gvhviongk.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/guxgrvrov.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcvnrfan.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gypltloka.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/guslunipf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxjiklqg.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gacoyrjio.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gnuvnddmf.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gyklnuzsk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpylnexk.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjnngfno.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjkbtziu.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpdmudqg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/godvrkpzj.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbloiuxu.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvgdhndj.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gldtgtldw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gojcozrgc.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdfbtfpdq.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiimndvk.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjdnthql.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gawgpaihh.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbnkrdko.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gwfchapqv.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkhcxemr.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnlhbyrb.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqpzlrai.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxjiixmh.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gutwchkle.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gniybyhrd.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gpgebdknb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/ghrxguzex.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbonvxgc.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsoooobz.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwugdirko.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/grsautiyf.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gifwadtwr.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gcoproxkh.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfesniqh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecwgrtuj.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gyajdimwk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjdsxfhk.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gjyekocqk.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gcadzmhav.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gofieycvo.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gvtfmilzi.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspnqzkqm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glylyrnow.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grztikxqh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gadjyuuil.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gulriimhd.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gmrjlnnxd.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvuxenwe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbzkpwit.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gcybjprfj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwqqrdeqw.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsgzapvf.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuluryti.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gaatobqyt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwtubtdyg.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpdaozze.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gueghdyoi.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkglwkidb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gpbngpxue.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gnpjrxcvn.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggclbqafv.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gxgligpgm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gttwsaeqq.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrodnhti.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gblrlceep.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gmirijkjs.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gqaquutdw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjbaejdce.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gxymzghyk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfhcyqjy.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ghuymjqsi.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gppykscob.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guuwsvnea.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucxjeiiq.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcqksehm.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvovxxeu.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gizdjkkyj.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqwjppbl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/grgxjzyhz.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjvbyczc.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gbagckqds.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gcduqmldd.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gtsytigsd.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnmfchpv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbvskcye.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtssmeaoq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdojpdux.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gxabymuzu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gypdqajxu.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpaohfri.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/guslvyigd.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdadewde.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gsbhivdkh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/ghmylkxlv.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtofqsvd.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqopsswke.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gmjdtbuic.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzlqzwwy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgageers.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gmgygmgfb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsxshcwy.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyrknxfg.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjzbntrs.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqpcezat.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakywrvrh.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpukwmdby.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/goqaytmel.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltjwflxh.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gszqkipgv.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gpslferfl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gvhpekslu.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzsxdlqw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdegktytz.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjslcsto.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gluqsahzw.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gyypumcuc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gzvrcroso.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyokfpmsl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgcmsfll.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gfcgawrnh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gorslxtfh.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gpvhyjpsx.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkseqyvcj.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gicpugdnm.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gbfmkvmky.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjghhativ.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfubnojhw.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gckyqsgnd.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfawuooj.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gejtzjmdz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gczdlwczq.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtuxdrml.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomizsjab.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gfrmvclnp.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkkczuom.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfcyuiol.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsjakkxn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhcppmmc.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gydarznnx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gheexlmyy.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gysefqjff.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjsegcdx.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gagdvqpsg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grqafpsio.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxkisetk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gdyntqglp.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gubbrieje.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbfhdsyf.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gytxwwvml.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gwcqqsvsz.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxjtmubg.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmyjcdka.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedtfhygn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaurnvfgl.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gcesduesh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/geqkpnmag.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsdmsuiut.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbulzavsw.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gywnkbrev.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gkopjioeg.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqqfztpk.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gjnavtfes.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gyghnofgb.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnarvqfnd.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gufwxwyix.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gmkgcvltb.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gjdntqhct.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsnkrydqv.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/groosnwuv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjhnmyje.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfawtlath.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzxdlywx.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ghquergia.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoeaqvhg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmerljjyf.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxwkhqio.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gpwawvtnf.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghifgrmwi.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecmltvza.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gdyicnkkr.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbovtmird.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gizgmmfxk.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcsdwlcq.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gbqwrzqws.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golmwehjp.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gztvwjyau.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsansrpj.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsykmeyn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdwwygjrr.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gslbkgzhw.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsnohcpu.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gjkuqvnbl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfrhjuvh.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzrvohtk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gonjkrldq.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgjtccdq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssiifsmw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gedatwbig.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/grjfsekso.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpurwgrbn.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gazrvztqa.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gtdhfbtxs.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzndadxyb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gmesgfela.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuqsdxhn.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaowvuzzq.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gfknniusq.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gexoggxod.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnegxqew.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gijcdebhg.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gmyschuzb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggobkiueg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdrypech.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/glicacqdz.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gsvhelifh.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gjakrjrxd.sHtML


<!-- 参考信息 -->