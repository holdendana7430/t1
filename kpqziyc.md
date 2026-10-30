代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gyohaxmkb.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoahltoc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkjpytew.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggzwimbbs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiudpdcj.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwxflfsk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuwirjbi.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gzjqoazwj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gaatnkkte.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxwmbxem.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ganxvwijg.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtrygitw.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtylhihow.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/godsmimha.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdtgghvob.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsomjxmo.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggidvlqkq.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/goekhjygz.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpeawhhh.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqomtiee.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grumotbaf.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gnejgnbem.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/guhfozppn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwxidgxc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gslpxmiqv.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbqkbjig.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gqpqsigkw.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoihmdxd.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkcvwctt.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckfncjui.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlxjmmsd.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gduiunxmw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrvtmmfr.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmxjgnto.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gprqvqlwa.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/girvkdjpe.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaigbcros.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmefouosp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgajfsef.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/guobluqlb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gwlqvkyvs.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjwqwznh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdrveolq.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvcmbjpg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtbqoaje.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbynjilm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gidfiranj.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gzjzlqhjn.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkvzpvsv.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatfpopyo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gjydsdqse.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gmnezxgtn.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/geromurmo.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviilpjol.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/glzvvrazb.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfpvpxmv.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gszypgmyv.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gplflicty.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqvdwlrt.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuwwbaxx.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gzvpincvk.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjptwqlfn.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxfmztod.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gystdlexr.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gbyouumis.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gzursbvfv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqriwxcy.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrmakuaq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/geobpxjcu.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gmhaxawal.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqsjsrjxn.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqllkise.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gjgqqclpt.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxpnvtbk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxlzdyvz.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjoonwsf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gnibqcocv.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpiduzxgj.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzrgacrhj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwnqlrxm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gesrgvniw.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvdplcsv.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjxcfjie.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaeyhgot.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gxfgexrve.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gdqeobyfo.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gkfejlrkt.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gfebijsme.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gppvojyej.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gorjofzyb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gjqkagaba.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmogdedx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gprygkugn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/goackdpzv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/glhkuhxcz.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gmopetsol.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgalpvif.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjaltigpw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcznrbdj.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkiamfao.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/ghsruujzw.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gasopqooo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/geogwgcaa.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzynvtdgw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gcueueawl.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcvipgfl.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gfpdylhwp.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gsysrbsis.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywgwmsqz.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/ghtpraplo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvhqlwco.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gtfpnuajt.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gttbeaqbn.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gufpohxkf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwfbbmms.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gxzvelhdx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glposolpy.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyobjkmw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzsdurlmf.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhphupbs.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gmkmjdfuc.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gwdrefcdq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gygwdyhag.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxoqefhz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfenataby.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpxykzjmw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gylelcwvj.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gablhcupj.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gftpxcxyy.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gnsglhkrc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvduptqyj.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiopfsrm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejpppwpk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdocrwip.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgjngqyp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/guivrpeys.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gmvfydndk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxhaoxhaa.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gnhtmishx.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgbutftu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsldmrtal.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlqizigm.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gpghahjzx.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gntfkyqwg.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gayzuqjmo.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjipjffq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gedbllpxs.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/getxaralx.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gcdmwsjlm.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gtesgvlvz.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gvnvnmdck.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gyknsekji.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gtteouqkj.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gnshvlhry.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gufeiicgo.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gzongmzcl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmdjisku.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/grzwevqgg.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gnlqhvnuz.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjzzyango.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/getomwbfm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxesaxaq.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdphjjahh.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gljnsraya.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/ggjfboqef.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/glzbycbhi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfxycbgt.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gniuiqqro.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gkujxjncm.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxruewzxh.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgbvoagu.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxpprofa.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqbxlvnt.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljqmsqip.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/grzhmlxuo.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiuikctc.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/grmiiyuze.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/guuxswhit.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/glnerltpv.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/googgdcwh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gmozibxtm.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gisqzilbu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgemmect.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gugyxtmjq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnmakkgl.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfrmhkhe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpchmckpn.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoufrqfg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gmbsmcpkr.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfitilqpo.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gbwoxxvqq.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhbkpxjm.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkdsgwji.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjsdjzhw.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqshrkydj.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grptgeayg.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/grcvtuola.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhvxykyf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqqbdmsg.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvwyayrf.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/glmdletkz.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/grdchkuhi.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrfipffg.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gdixmgrkq.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpmrwdmp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwjjsklpz.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqjoscoy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfjngkcu.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoqtnxqf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgmxsipx.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/ghvieizlm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkolducl.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gigtkweay.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gldqwkrni.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gzujfxlzk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/glhkyuwbp.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gutcdbtff.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqpiuapw.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcytjshj.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgqnpbhr.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gcryymgbv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gslspfuxp.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsenbllpx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/grxkgpkwu.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjmcjehe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gsysevzcb.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorteqnxc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwklhtzs.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gybtsxaai.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gelfsewot.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gceslkvsw.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwriikwnm.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqbrpppq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gheqlczju.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahnglndn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glkenggfw.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gwliwfgkc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcnmbbxmp.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaahtkit.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdypwunsz.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gbgzdqhdt.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwpvrjdq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvhtbbtg.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gjrsxrmtr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjfhjzhq.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhqjseeb.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtduexnl.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/glfruoyir.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjinfnac.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gmhszxrmj.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/glzyjipfi.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gltmyofik.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgcrhwbh.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gomspjnmz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpsjkvwn.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gnllwrufj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqghovth.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheukmsmu.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhtdgkfl.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxtxzzct.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/goaklqkrt.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvuabcjb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gizkwuyqr.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gynlastvy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqqgnmib.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwteyldpv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gynaqdzuo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guhzmsequ.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gqkzaxpru.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/geylegojz.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegnyqqdp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gsswheyqn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgslihyl.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/ghtnmuspf.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gevvtnwol.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gtklbddac.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvvukgyn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlaccjzl.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gfrdqkdao.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gsitttjrt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnwdkkkb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfrwqgqp.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/ggooklkhm.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gorksnhcj.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/guxxjugue.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gfvwgslbg.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gblqpcgxt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwbhzjtt.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/grsiwmtbh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gvnazfigd.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljszpeim.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gafwcubas.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfeapeps.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxloxksrb.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gycknneqc.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gziwxsbvs.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gghadsrwp.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gnwqvawcc.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gygutxeix.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ggzmyyjaz.sHtML


<!-- 参考信息 -->