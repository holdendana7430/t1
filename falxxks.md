代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghnvwheza.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtgtikfq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngdikznd.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepgvdtzp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glhzssflx.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdxikrkc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghackltxh.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoluwtaz.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvjyxtyzm.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gdlezxrel.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gnzvzqbgb.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfoefkob.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrczwpem.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gseqrdplt.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/goehwfzqy.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glugyrfqs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gwtndxugt.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gatbbfcmb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/guqzxeyix.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gdokdnzqz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/glgfosamj.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmgetjqd.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gilvrpcei.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusdmiswz.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gxdmlmltu.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/griplpril.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/ggkbbjbaw.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaswyjph.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtpblmuk.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhjbmspb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjrsbsnf.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiwakfvq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxduhkap.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/goxpxpkhs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzwcutiu.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gpciiyskl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gbffoveyc.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gcppcsqmv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/guipzyfez.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gntydefsn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gspxrcioy.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gzjgiwugk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgswcghr.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gbhjwvdue.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gctjzkvhi.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfgqcxdq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhxfjwig.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gszfxonex.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gvqlbfnxj.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gmolvheoj.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gktsxzqjd.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsikpcvg.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfugnxlj.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbanuewti.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/giidssnqu.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcoawnxml.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyybjdns.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gqexteuwk.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/goztavlwl.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjjqwmfc.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyiedysv.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujgniszd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqctjocq.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvgyhaiw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdedshkxo.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvyciktv.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkryqlsyd.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzwvvoxj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkheildr.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkesbeiw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggczefrbl.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrzcinpa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/grdykqajy.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gytlxdryj.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkkhgqjf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdcsmmji.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/guzftjztd.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/goepumwpb.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbakqqgwp.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygtyqoig.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhrprusa.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/grlvkrydg.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswdeopcv.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmcdojot.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvakjccj.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxboengt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gfraudfeo.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/girzkfglt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geojnijye.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdluvjhn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gkuyjgeta.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxxnpwke.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctfqlkni.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcwnvoxyb.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqqncmma.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gjvatylip.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfiqtctt.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnosugbr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaupjvhe.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbazvuiid.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gvifivlth.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gkgpamozy.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gebtwqxle.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwelobgqj.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/grwlpxrsb.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqidykte.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgyzwnuv.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gypknaryj.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmgppvwj.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbeicrmh.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/givuiczeh.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/guzxgysau.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gkonjizip.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gohqvgunu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/glrdfzlia.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gjmhfnnnn.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkykqgzmi.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfufceew.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gntemieex.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gezeecfpf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gzfqajyxj.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtumnflrm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gkstsubrr.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvaowtvo.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvuvsynm.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gghtbwwmn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqydbkdsq.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/ggaqpwkml.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtngucqgd.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/ghevxagxn.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzskksft.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnomrgtzu.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gpiokkjak.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcpijmxxs.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gurlbhxhw.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnvqslvd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/giujcvkbt.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gltiajwuk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhtnxzmc.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gryyjmcgn.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjeyfmjab.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmnusgrr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzghxuwty.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gpzibcgnr.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyinbifmc.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoogszax.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gltholxel.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/ggnjvkrwv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqfnafjv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gnevzdtun.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngvmauqg.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gjircgfmr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrfxhkon.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/griftlohu.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/grzwwwcib.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzvlxhhc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gqraenaiy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gglruyseq.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/guayuzlui.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsrzecdm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqmcrane.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/guyfgtseu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdekmwgm.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/glquncgbw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/grjqqdmmc.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/goafaotpk.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gwafgttwb.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfrgybue.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvloozlh.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdnhhmsu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gouunqvlx.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozyilsff.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuhdetju.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsndnbkuo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/grpnywmww.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseovshzw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gvvowvbmo.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/glerxnkjr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzdpdvpk.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfrjneqp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/grviohdvi.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijfeqgcp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gdaarxuuy.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gqupvdyma.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnskplho.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gpdzzgjyi.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gykotezum.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gihwjmwuo.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcrqbdqq.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmkaisqw.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gueyshgww.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/grunmgjgp.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gyhxsaafc.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvsonlwb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtazntqqo.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpkzirbd.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqexbfrue.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhmwpmvr.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gagbtpijc.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/grhazvbea.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrnrehwi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gufshjpyg.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdiddjml.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gvzrplgce.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gkquzokck.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsflesfjh.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gawcjdafh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gezaeskld.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gorwbwqks.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfwobnuf.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gqndfbwvz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gdfpdeztk.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmgloofx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbtvziii.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gcatzewdw.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gxojbstse.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmvtgobl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtowijcw.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/grglaahtk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gpypcqtxv.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmvgdyrwp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsuwsswp.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxhtxfnzy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucghrpwl.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gieqewoew.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqptqqmn.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gxislifhw.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gemufzova.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/genuaekfm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfpfcmmi.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/ghdozjozl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibrkmszu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvyrqfuu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpuhhagzg.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfflicvoz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gppvhjftl.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnauclqwu.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsenbzdz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqcjonsz.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gmxdiwnww.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmohebpq.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgsmngfb.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gxnwopcqz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiibzgby.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrfbnaui.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdqyijng.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcdtikrf.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gdtyatmwt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gitrjojlf.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyqzhjyr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/giqfywnbu.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmflnxqi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gytloirgs.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuuprxhw.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiqsqfgx.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gmqfzdbok.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gjaboxfuq.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkwrbrhi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlyyvgvi.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/grkxlualf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/ghdsfgjvw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/giqapiwyb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/geotddtys.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggisyzyqq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ggcyxhnja.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gakqmgxug.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbacqkjfu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gsfcdhqtu.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/grmsdndwf.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gxejrivjr.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gotiknyyl.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gvzpzvtqr.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/ggydolocw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqjeehfl.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gmeudbibx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gnupzcjup.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gqsskaeay.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfskesgy.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/giixwpemn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkvsbtjn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnbridjm.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/geuznqgwe.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gijhsfbdg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gnqosrsrb.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/grgoitmtv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdytvtyec.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gcozbngwq.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gopsrdzod.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjtpqymn.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzytsdes.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjcoshsh.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfuympyf.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvqsygdu.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtlkivtq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrxgjzje.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gwxgeeyaa.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gfiuuwpru.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gnvqsotrt.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdittzftx.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gsksymhkl.sHtML


<!-- 参考信息 -->