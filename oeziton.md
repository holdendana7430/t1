代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gectqxdha.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gfojgwiwx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbhnlxaa.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/grihuqass.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwlskged.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gipzwpxty.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gwmaggfxm.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvibyytu.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/guhvodgot.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gofifoqze.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfxszmnw.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gthotncjc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiprjctz.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtornxpx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gomsoeiiq.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgngiaai.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzftxenof.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcbkkwpr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumeczncn.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqgusazt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnrhnbdb.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrvojrhw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjrlzrsh.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/glqiohvjh.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzrsuydp.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrhmtqjy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcjkmtmem.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqirwjlk.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdfdfhgp.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjylbhlx.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxtglgqt.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gwyufucmr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvlkgfqc.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gedatcvyk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehsdwlrt.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/givocfknk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhaozfpu.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsumuxktb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmriuqhox.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchmtzoug.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gfrpbrkui.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgczppsa.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxfdnfml.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqmnvxzpw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gawofpnrz.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfrtcudn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/grjvvzprq.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkzefcmly.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfwgzgkox.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqnjmzvw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkajwvhlp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganmytnqb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gonjexbci.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gvyrncfkg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtstxgibw.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzlvpval.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmokrhtjs.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gbkcqgbgr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gthrpeamr.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbgtybdp.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvucuenrc.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/ggexfnmcx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiqjtvjy.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuwcyagl.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmlrxheh.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gppmxljqy.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/glpcjzmrx.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gdtnagifm.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gwcevzdpw.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gjvldeoaa.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gsjdtwwch.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcdltmljb.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/guefobfkk.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfhxdxdt.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbeexfdl.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomlsznar.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gkfccqdrs.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gjomyjqmi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnqtcqbk.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmbfraho.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhyhgsxa.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvifsoqk.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gakbxacgl.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gulnkwdvg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gyvksazxj.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpqfetza.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glnrumtdf.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkdjkuap.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gprukmgam.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcicmxbsq.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohwetlao.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gyloyzofi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gpndctjhu.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbpswprn.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvonawsei.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/glihmaefb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliuudnla.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gezbifbjy.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdrphzru.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcpkskap.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gtvrzqosx.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcslpcwr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjxcrwuk.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptgrqlsz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/ghvkuhpbp.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhbebpno.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvitvmyp.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvisjync.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdddvbdt.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzicauczf.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gkyutptva.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjuzqadb.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gifdnqvym.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/grpubvpxo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnogoydf.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gihnxhuer.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gmistliov.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gxigcmtik.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvtoevrl.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/glhrjnuon.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gjxdkctcw.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfegixvhu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghnwttgwa.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwefwaab.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gezobnmfs.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/geckhcksf.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gcbpvtzaw.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gtfhvcdrn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gcjgzgaus.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gnkmkhvej.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcbictvli.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojlkojvw.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gliyichop.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gxecfdhbq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyznpxze.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gdbbsbqyp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrjexeaj.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqkrcajna.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrofdfhp.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfwjnbtu.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpazkoai.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gkjdpomde.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoxlyihs.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/goeivyhxp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkjnrirv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerpbjuhc.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqxqmeuf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsjxvmnuv.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gnywypqfl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gclsylwtm.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gmffnzdow.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkalripy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhyetdry.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmbqiuhy.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/glgieeeub.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gxxflwinz.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gxrfaqltx.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcstcfsv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliaujpsk.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gcyaffbzj.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gmcwwmqdl.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gvbxilvup.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gtzsqmqpo.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gnqhadrjs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gaafucphz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gorrffmrb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcqqcqva.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gukeuydrr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gevcnrztt.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gkmtnwqhm.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gxjqqqdpm.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzttwgqq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmqcinqt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/giytwtqyv.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiyuozyg.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glnbivqwc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsgmhixq.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gmcwhwbmg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqrduzha.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuzemafo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjzbvdwz.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gzxxohnmt.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gglcoiqgq.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbnqrxxa.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gfdswedvn.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gostppnhh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyynamphk.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gvupvznna.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gqjleqpnl.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcgbcubj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gojvmfmql.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcgijoya.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gnkvenrmz.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/guafxtihr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/ghbrglgbh.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gmrmkdrzf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gsqjgunyv.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewjyaciv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuefphtr.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/grfnwaygy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gacrxsleb.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gixvgqasy.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gcguovknn.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gamonglzr.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/grsiytztx.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvnhwkna.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnwusbok.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gojijyjwp.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/grtkngcqj.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfmaycuh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gastyauqj.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/geipnadgl.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohrglvrp.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/glqcazvjw.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijynixox.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gtgkavmae.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/greuonnek.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfusikpn.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gpakrzvuk.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gckgrvwuo.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gvfvefvdm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/givobkxyy.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gesrbiqvy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gykivapie.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gumcrrkpb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmfvgbkr.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrpjufet.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmdiacue.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gllgphljo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggybrxoem.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gikfnfpeo.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gowzobwsn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnakizawu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/grukuehjq.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gnpnrajnk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gsajhryla.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogiblvxw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqpkrcab.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzeyqapi.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gyccusyqf.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjpylznw.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/ghpuxxrdk.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gxsnoyyka.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllstjqju.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/glyfnjkzh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoazdmmg.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/glheuyegc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gywtfbfzn.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gabvbsowa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gawmxwgyk.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggecfjyxk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gixzcphxe.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gxdkmsqvl.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjmratqyb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gtqsjwmfh.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gpfnqzbcp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwznyljbs.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gejrzqiik.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gtcdbzqjp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcanogqid.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvqnzgks.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgoqngez.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjycgnuv.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxulshgsk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gnxxtwqzo.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gqadsthtl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswvnuhkd.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/glfmncawc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtcmsdpz.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxgnidwm.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvsjnonw.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gtsspxych.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gsqeujifi.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgjrpcls.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gigsjildo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrxoscyw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrscoxdt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsswgowm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfbpjetd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgrpmwva.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfklpmedw.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtngdvlas.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/geetfaruq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gidgxmliz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfttixvjh.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhjpizqt.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbfwvsxb.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gnxvkraqj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjupissh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpsjwauq.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwvnvbgf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gmcvtresj.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gvarxmtrt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxseuqbh.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeppejdq.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gypwuinhv.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfooyaxh.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gmskdpdbf.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gelmqgbtd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gedeynqqf.sHtML


<!-- 参考信息 -->