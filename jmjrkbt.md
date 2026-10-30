代发 wailian999

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdlvdrqx.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsonzmjh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gagjyjxmw.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjlcqobi.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gniopejnt.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gsquwitlx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/geflnantg.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpkfhwlti.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gnzmkszxx.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/grsffxgaw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/geqdjptdq.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gckbmqczx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/grtjyuety.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcmtoiys.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhwoktmd.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gikexiakz.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gfbjpnhhd.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcaxhrzf.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gqdiceoym.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gymqnfulf.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gojplbhub.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlotrzjo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlgetthy.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gryzqaney.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqfllkvq.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gekwplzqg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbamstmm.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbcaeewz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gknalpblr.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gymrxtwed.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gansxvvuo.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gzrziousx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwvhiroqw.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gtindoatj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcbnagmzc.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gtrhormgk.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gubzrpqrz.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gyjyzelpo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gxtulmxow.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjdsdkbn.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghtxlnwru.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/glrccyrhc.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgdlvgyf.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gztjymsov.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqutgcgkc.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gilnniitm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmamlzdu.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gixbkdxev.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gixcwfgbw.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiaygsyy.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnivrtysn.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gordldoss.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmqhxlun.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gvblbvlfc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlftrbed.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gozgusyfl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gcoeqnwck.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrjaqiye.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzlqdzqp.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gszruqnpt.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdlucjzoz.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gydevjwzz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaouhjnd.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gvnajbymr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gyelwseop.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gstxqqyer.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzwapvnj.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gloxppldl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqasqxvs.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gpczvspib.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gythwdvzq.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgwxkthx.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geskynedo.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhgcuejn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxhzdtlh.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gyibnnzcd.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gzinctpbz.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsvbnmol.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrtgxxsj.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvqkpnvh.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gxlvotekb.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gzaqhmtni.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmijebczl.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnbnkzjoo.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoqtbgjj.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gnrdqzdfr.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/grcxwmoma.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifenxkwj.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhjybkaj.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gvbtrgkod.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gnszdmbmp.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gouhpzbrj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gftaeeavq.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmmsgrox.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdggusdob.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrikgmnc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginsewjqx.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gymmqwtdd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggqhbsxmf.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlxjicnv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/ggpqlvdbk.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlbxoshy.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqbtpups.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsvggnze.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gwukmklki.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfncjzkph.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gmnjwoxjg.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/godfmkqbi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimjxekyp.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gpftcfbra.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/ghakdojib.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtimlnpf.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/glqtpzzqu.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gykxhfetm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gpliryzyd.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvsdaojp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/guxzalfla.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gghzncocn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfehjxtuh.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gwndyzmwt.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gxozhyjjs.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeulzmmr.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuirmghe.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/goutvnxzy.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/grgbkdnje.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gyhwufvto.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpwemtmz.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsnrxzpi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gpzmtxanr.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gobfatcvk.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssztdxxg.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gqjntuyln.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/ghlhlaexx.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gfajikzbp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqhrfmxv.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gfloaelqu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsysdxloj.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gecpzxtwz.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglxpkhny.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gvqvbcbgn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/glumviaeb.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbvjoeyd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgtpphon.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gdnoxoegy.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlzjlaur.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrjvmmll.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gcahgkyvs.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gphbxfxhs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdcoksub.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjghwhjw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/glkimnear.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/glfhqqosj.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gkitflciz.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtdogyuz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqctgspt.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gnybdrisy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyqqcvmeo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydrftgum.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtuucvmv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldzeiuyh.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtvyehlj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glpzsbtyd.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/glzyxmawg.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gnuplejvd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/govpdlgku.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/groljswhq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsueqkqe.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gmilvskje.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gvhshhqps.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwizojke.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomfbiptl.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gtjxagqnf.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjcegnfy.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gztvmwjrt.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gddpsbgam.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/glkjgfmri.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gsbivuvdl.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gzwijcont.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjnnqwmf.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gshfedmes.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/grvkxvvpm.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/geajeuagv.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfriszqsv.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/grwbugoax.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gmjygkyrb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/goylrmvlw.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gantwzizv.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkkzwajde.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/ggqcoixap.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gxbzxqdvu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/guwosthxi.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gmryrqzxi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gzvxwkcls.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gttanzrua.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gbixenqfm.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfxepuon.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwagneau.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkdwsilh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvscmxgb.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gnbpyvpxi.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzffxvsjw.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gqllzcqbv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrlnfkxx.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/glhqlixbz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnlteivx.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaywflci.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gokadkcbu.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gskbshnpo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gcoczimcn.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gmfcniwkr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbdipgjp.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwohhizm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgjbipzy.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtoxwwlc.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/ghatsrmaa.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gfrgeqaig.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqqzwvpb.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrbandim.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gtbljtowk.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/grfaajcnj.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjkdpehm.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjxmalyf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqozzwmsc.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrpztjag.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjendqsg.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwzwgpob.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gjjdwspbz.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gshomcgyu.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzmfqyfn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzrvayfo.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyngnrme.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gswdcjunt.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gpezrcjat.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrvmgldq.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtplfwym.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlcndlcp.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxxmxzho.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzldvcejx.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gbuoniqnq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwjeiavwi.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gzjfrtnsw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gpqevjncm.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gsiuqwctd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfkpwgvq.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/grzoczdvi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gpdulbkab.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmgdhtdt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/guvolqumk.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtjzbackj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gsngklcvn.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gomoljajd.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gtleitzan.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgvjtbad.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/giagfgcgx.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvpgenqm.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxczqnqgv.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gizoxxqot.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/geiycjmdn.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gfucrbacv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gulvbnsfs.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/glfgselcj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmqowywm.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gecqpxdey.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gdjpskfka.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/guqcvovxs.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giskpdsyk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gudtyvymo.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvnxmhsv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoumsexk.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxgxwiifb.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gloxvvcyi.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gsojwmsne.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghmzhekz.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gbbbzqcho.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbugfrpr.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gobrckmlc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/glzdcjszn.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gzahylprt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzolhgbqm.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gfstcxmcx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gujibhxsn.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gbgwbqotf.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwylwogb.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/goecornel.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gslbfujft.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gbfzjzshy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrtjvuce.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdhfwyew.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gvxjkwqgc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsjaqmbb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gybclspru.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnztvbgab.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gecmkuhyp.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gogwvkmfu.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggtddjjwb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gcrtzwwfl.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gykteeind.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhctrdgz.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gezmifxvs.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfhqrrgt.sHtML


<!-- 参考信息 -->