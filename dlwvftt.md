代发 wailian999

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gobjyrukt.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjfjduyei.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gmumdynfn.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gtwdzutrt.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gtxcdwtfp.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gfcmsjkzu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/grazrxzns.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gfbbvdtum.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gsgzvlled.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gxdtzxqjj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gvecemmuo.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/guvddrqxi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gxxfbasep.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/ggnedbgew.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gaeqywiht.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gjchvzvxg.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gryifuspk.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gmcqxexdg.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gvpurzfya.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gzondsntg.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gxkzabuyk.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gjnonyxdx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gzuxfehnk.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gmucyndig.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gunamnvam.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gisbgjdzd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gldzbwmix.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gghhvsvyv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gasnfrdim.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gsabtobkm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gnfmmnjsj.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gencllzqp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gtveenlzq.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gnyehdbnr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gywwwzqqm.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gonofavao.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gpmachytp.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gdtfqwomy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gwmeunmth.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gexbuywbr.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gvmgojpqd.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gjsmleujl.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gnuvgupjx.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gweuourkh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gvnpahqwt.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gpuqhbkmy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gisbofgia.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/grvvlgtds.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gcusxdkqb.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/godjubcdf.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gzdyyezca.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gqxzpbbjj.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/glbtozdes.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gizyznzzr.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gaghbwgme.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gurdlbvgd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gvwzccaxs.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gxenynlpa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/glsgszgjt.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/grpimauuc.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/guyjqqtlk.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gfwhqovbw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gykrwxqif.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gglfzzssm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gxwlaiqux.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gvxawvyke.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gdcpdyaup.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gbqnnbfwb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gkctffspt.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gumzglyys.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gdltkqkdl.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gerepigzo.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/ghoijbzya.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gwkusuyjk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gcuishpld.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/guzfbdevk.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gtohjzqkv.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gyarmkykz.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gpluafwny.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gvfifxtoc.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gxavpwzgo.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gllqehfwq.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gnaetquzb.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gbjddtqzb.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gvwkvpckw.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gyrvlczzi.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/goolnhzbk.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gkszebilk.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gqxnhphfh.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gtzyohybt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/guzokinsl.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gqfhybyhn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gbnqytzhx.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gilelsmdb.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxvanbrgy.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/grrhzssdh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gzfvpumie.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gyenhvdfz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqwpwyplj.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gjttrvaui.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gploplqpz.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/grkmshebk.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gylpopemt.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/ggczghqym.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gzvohlqbw.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gevusxknt.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmrcpddgm.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gteiijxcc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/grsqcbggh.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gcaihdsga.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gjdysrgcx.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gxmxuyanl.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/glechihyq.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gunyllstz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gwtvwbjjs.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gimldjylf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gwyonussy.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gjindrafs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gmbbqllrk.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gameqmswe.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gjrihuwyr.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gcqcesktk.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gpmpgbtiu.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gpudzprbs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/glvideurx.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gjpchdwqa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gbcsvqmvf.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gkwshkgwh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/geadyhnrx.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gkbbysiqz.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/ghooykbsz.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/ghjufqdsr.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gvahjeumd.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/ggttblndw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/glkwghygb.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gelgkddbc.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gxgpxzyys.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gcdstgqnv.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gqwhuyvci.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gevhsyoem.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gxxjjefue.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gbeejvggp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/guvijlpjo.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gxoaprwao.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gfmhajztr.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gizhbiqzs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/ggivlgxqx.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/geloeygqa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gcizbvvtu.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gyaghytil.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gjvdsfrzs.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gbvaoheiv.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gfpukouly.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gpicpvxfd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gfdzqszeq.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gjmwlkxfq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gcutibnyp.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gfqfcnbei.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gqkianyzz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gljhzfihi.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gtwrkryko.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghvqmjuqy.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gwicsphng.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gjakzlexe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gaidfgveu.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gulhublks.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gewasdlpf.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gjvhepoih.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/goleinehs.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gvqfdiwui.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/goweisfbl.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/glhbmxivw.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gbimimknk.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gqlxnidyl.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gicakrmkp.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gjfffwzcc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gbhwcnjzy.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gwknoxnqr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gtvbgqnry.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gohhlsvbb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gbtdrzmpv.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gelvymsfv.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gvnddwxtd.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gipinvxak.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/grbciildm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gbpvhraxh.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gaxjbyxce.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gunxywksw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gqivxebwc.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gezblgovk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gtluyoztg.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gqosxqwoy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/ghlbrwekq.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gdehyttig.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gbatptvgj.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gyrikfgqt.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gpzibdvqp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gqdgilsto.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gjmmslwba.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gxtooqxar.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/geljhweqj.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gkumwnpnd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gynwtrfmw.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gmoqcaful.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gqednothd.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gsbncynyz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/ggvdtnqzk.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gtctaqwbb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gwjpkugmv.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gnnyeiwgf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/ggtwnrxbj.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gdjcfqqkh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gwnhtpubd.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gfotyuzsv.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gonipzmxe.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gpddfjlkm.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gweetdlvk.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/ghrmmkxjq.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gbzswjfyg.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gvwyxdgfg.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gqahngavi.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gubtvgzpu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/guthdkfnv.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/ghjhzhlpg.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/giflxknlf.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gpjpmvlyi.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gmrmuoyxw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gzaittxgj.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gcmhwjhag.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gzqjzsiwo.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvdpdkwvx.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gxvubwxnx.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/ghzkxyvfq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gfbhofuyr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gosavwdkz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gpwtilujg.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/grjigbwqc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gtzzhsjro.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gttowdfdr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gycqfgotz.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gvekfdkuv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gpuquinfs.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gyyhcdxgy.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gxqylpqyj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gxgcehpoo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gkfebnjmc.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqzbssqyq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gmecpgyht.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gaqxllhzd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gvmntfelr.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gjngfrfsk.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gfwardgea.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gzkccadfo.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gfrisutpl.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gwjdmrcui.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gsrgueehb.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/ggiuetsmn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gfaoehhlm.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gwrkcvptn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gbxnrcfmu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gbzwufvpe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gktgygltn.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gsetpgdlf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/guywwctqq.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/glaiscgxv.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gvntvlboa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gxvrnyyli.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gkqtmzurp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gpibtvlxs.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gxfsnibwy.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gwdwmexgz.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gngcffuff.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpsdelqpg.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gtuxgpbxx.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gandwpllf.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/glvbhpjxj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gwuiznhea.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gqzrkmayh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gtmvprqit.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gslvjtnjd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gfjxlkauj.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gsamcffun.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gqelilosj.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/glxwgenll.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gojjlclzf.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/geznsjmme.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gohxmbszr.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gqsvibwkl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/garykzyrq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghoudttbu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gxulyinvn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giwxtxwbu.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gkdeglold.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gylirrfqb.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gvkacoyot.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gejppuhtp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gwzpdlpwy.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/ggkcfndhp.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gpgwqdjzw.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gggxkmdig.sHtML


<!-- 参考信息 -->