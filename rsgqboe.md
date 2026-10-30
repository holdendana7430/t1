代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbqrzeww.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdazbdlqv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ggkmvduds.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrrabare.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboeuqaiq.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/ganmvhbxt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/guxoaiwgu.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gidzekwyc.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gwodvanpc.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/ggdvyfltm.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuspfjvu.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdahbuos.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpgxsymq.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghhelhfa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuyqrqoc.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/glvqinceu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gukhtznxi.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/grkzpsuak.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtveevuvl.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqoskwat.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gsesttmgl.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxxmtteg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzuqbipbo.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gnbuyfrax.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzdrpobq.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczrbcutz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbkfoauov.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnyrckup.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnawemecg.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/graxofayb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyulvwmuq.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmuftvph.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnyqppmn.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgszdgqk.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqzzabwfz.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgjfvwlq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gqibjeyzp.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtgsnngt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdcvhbyc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/genynmpth.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjnzlnce.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkjyxnls.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmcmuuvu.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskilinrw.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/grergfvyh.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gwigrdcsp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/glsxiifuz.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbelixsxg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/giiaaxyuk.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/ggqwegbec.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfpjxuhx.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gocrhfrrn.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjcrpjfbh.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gxohhorgu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzefemarc.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gaapfbrgc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gpexiozbg.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdytdoid.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhidakzh.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcsdjwcj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjfexadf.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gqgdjfjvt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gmbplumfu.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gevqiajgd.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnfdqgox.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gsubexncr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/grrobugpw.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkaqzvfh.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gimzlusvx.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgjzkbdv.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gilyrwlng.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuedwwzd.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gevblfunl.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlzqodde.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghsakfxnj.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gagfliybk.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gpozncjpr.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gwjzhagmb.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/ghgtugecp.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giitlefiw.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gwbrflnfe.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelgzrjyj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gmhrivbmj.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnplejrab.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxskrifn.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gxctxwjdt.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvawfkpoh.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gfwyyllcu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gsvrzcdmj.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/ggqgypyjk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjnckncr.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuxdvsaj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gbqdrzrgn.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gigisguwf.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gsclhaasa.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/ggxwntpny.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gdqduoaak.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjmjjqoue.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpqaoykn.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gnzpbtgeu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqpwhrht.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gpoyccssp.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gsavugvul.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdsmvaua.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwcnjrjs.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwxtaftt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gxxgzzhdx.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gaklzliwt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/glboicmvf.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gzsuygpgt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gcrhtubux.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdaxzfvh.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavltwvip.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsszgtakt.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gvugjrpai.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gzjdonmrv.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpscvvjg.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/ganpeolmw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/ggrdiehix.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcapbhyo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/guhugpxtn.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/goeypfksz.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gjxwhpvth.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghobcqfzm.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/goairwcro.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvazfkge.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gczqypwtv.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqbptork.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gohetocga.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gwljfisgg.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gfryssywo.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gezahpnfu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgdnkdyn.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/glajefyiv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbvbqagl.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gctjrpnsq.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/glgylxxqo.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvundbut.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtclhzmvf.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqumxzwv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnsyauqc.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwiujgyeh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gseffoojr.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/giodtnfzg.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgliqqyw.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/grtzzmaij.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdctsuqpu.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcammbvvk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrtjpzrm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/grduhoxhr.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxdouumx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbtsnqbt.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqymtesv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkwkgiok.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbffvifc.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/grftexuob.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gauwglyrt.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/goaqdkwdh.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnzwnade.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gciuhcwqg.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gficjumir.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcggtikt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gtqcxzvyw.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gcvarxxuh.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gewwtnevl.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gtnzqcqzy.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gfkasqbls.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gmybligac.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/ggxmhwhwi.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrssmzjy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcjtifis.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gpjajgkcv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gdzhtvgnt.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gskccsorw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjrwpclt.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsfddmbco.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/glqfukcqs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gwhhdqtxz.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkcsgbkx.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdfommhkk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/guwfkzyck.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxxudooc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgafjoab.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/glxundjfa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gvqrcrzpg.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gnkhvhish.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gmfhtmmps.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/girixozwo.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuxgoixr.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gxcuepikr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gvsthyxvp.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gshmtwayu.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gowxdxjhu.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gascpkcyi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwpjhifj.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgmprxew.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gutovyovy.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gsrizbfuy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gemjldkst.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjhpwccm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgbtxnbp.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcllcqtz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gkscswjms.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwpehuol.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmqmdviz.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/ghijnwxdt.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfelpnulx.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/guxihnqsh.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywsuqfxr.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gvwklemyy.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxwifzbb.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvqnmixxa.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxyfjvnd.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvagcxycs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gwmdnqpqf.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gyyrfgswy.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhvfmqtz.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdbhwspf.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfchncrp.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqqnqguf.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhcssbjo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzkckivy.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gdqdlrsfp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdyceskf.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkinjxqht.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goncnlgka.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafcnpxnf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgedocqi.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gbjgrutqu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjrizzzu.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gzlaoaeti.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyhgyrip.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gmatasjbi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaefdndj.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbgnexwg.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gaugfqqzw.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gtbngrpxx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuzwwghq.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuvbqfdv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gszkgxnxp.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtxkktolc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfglvwaxo.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gutbdigwp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gbqaqlcuk.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gofbyeppi.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyaigeyh.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gbzegfhfo.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtxgmvbq.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gsevznmon.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjceapvj.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqqnjtud.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaqdixbyg.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gkdtmgbve.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsjtiyloi.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwwgvthf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzrojehj.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitqkymyb.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqhmqwvmz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbsfbagw.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gjintserg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/grdgypnya.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfdubqfd.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/goinwdyyg.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gvlhfndkr.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkewnftrd.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmvuwjou.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxzmbgjn.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfmomsty.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gxsylugiw.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gdqjsruyb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyvqjisk.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gztmxpmls.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwcgvvzwn.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyofdyed.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gtjqnajar.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gpocbnlgq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfjbucqi.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gouwjnmlo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeacevct.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynhxgnnm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gfkjlxkga.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gayiqrpfj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gbgfpmxzk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gswkjfkak.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhlvjszg.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesbyqidj.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/ghxdsgndy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gjfikthsz.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gnuzulnxw.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/grkqymzen.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gilybeuxf.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruitkzym.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/ggikkasvy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwhqqqws.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gaoayypan.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/goghlrmhh.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gyawiaelp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjmxhzbr.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoxkqcmt.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/ggzxhdwep.sHtML


<!-- 参考信息 -->