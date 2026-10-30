代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gbombctsh.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gymqdsvlp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gengilbgu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbigitavl.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtsvuzwe.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/goyszivmw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gjufbbvep.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gnfrtesgk.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqgrqzoq.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgwjgnrb.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gzipdpvjh.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gltbvreni.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgkkegzh.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgwgfpov.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gicheqpck.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/geriieovx.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkszmiekg.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gzphqlidq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiipzmom.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcggolya.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlqcfuqo.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gkecqtssn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gjqhnqasy.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/goibubovj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpezflmi.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gtyncukjl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gplsfacds.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gavmhaczk.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/goddlrfpg.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gzmfmouao.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmywtmfch.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gldcefecj.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/geppnujmk.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdndcbcdp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnglatwz.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/ggloqfkim.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzuzxyan.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gugmgsqdg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhtnskgp.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqybpziyg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gguwtfjnd.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/goutoaswz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcssymkl.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/goiahhrpj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgyjdcap.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrytfets.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtrkizflx.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gzqzugmon.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyvubytj.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gecunwozu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/glatwsqpx.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gpaihlpvc.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcqmisfj.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gyntrdbir.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpdspvpb.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gwjgbqces.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/glphmndja.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gltbyuggm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/grbvzjnvh.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/ggmknsbmz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwldipat.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gntqtgxqg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girszjcbs.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/ghslwlfhc.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gvnxdysjn.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/goxlsrawl.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhcfyrjr.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gghcxcjof.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuspjele.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/grgnrbmwl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqvyyyti.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/goysfoder.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghvlbpmcc.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwefojna.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpizehdkt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqkrkhnz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/guifjyeke.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gcfjoylsk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gladnegno.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gclfhjhdc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkvbnhbv.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeouvrah.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyiehjwd.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsshjuhkx.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gbzdmdstc.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gdexjxrok.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gokhhzwdi.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaogcqeto.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzjbjlry.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gtmdkkiao.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmoaxnwm.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/girujxbsg.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gfakooykw.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gslnzkkss.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grnukfrtl.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpyfaklnf.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnxtodtb.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtbuskxh.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypvwvxze.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxiaflxw.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmvcgtll.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqunnsrq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gdmeszwtb.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmcygtmbs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmhxcjex.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsowknxho.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gquxcptsl.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbfzyfcl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gndjkxzhi.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/glixdfqxr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvbdgphic.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqurunum.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsweyyvd.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjkgjzlu.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprtgjgem.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gxfjhlpzh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gkosmylmf.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvrwuwnt.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyjqufgw.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gxwxxqerr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gledfanrt.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gxvrbnctk.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/guvqifwij.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpxdhjwc.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvrrjdws.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/guotqdnzt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gkceontnl.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzwmnbrz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gfguigluv.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gmpumwbbb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/ggjjhwrzc.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gkbjyrnsw.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkdydavc.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbwyuocj.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gjwxvahmx.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznpwptom.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhcsrshh.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gvdshbjyz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gegazzubq.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsedbsjcj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gngkknpxf.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmfqrrmg.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuzidmnr.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpgielsw.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gucvlmzsy.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/ghjgrrhte.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfhwyrrax.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gqiqxhgfh.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/glddsngph.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gbgcjobja.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gebcezdse.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgehtjat.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxsglaqh.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gmterznul.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gblwfaowt.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrtbjxfi.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gvvopnuih.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiyduszw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkzlcmbfb.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzrcgjau.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/glxnxnbof.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnbfdurcf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gjidecnew.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gebbkofoc.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/grkgdvcos.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkpyukvv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfpclqlp.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gnyuavanz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzmhoxzb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjeckkgc.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gaetnpljb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqqhbkem.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgbewudr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gthmvtsma.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtufdxed.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/ggiwkvntf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbmzbzbft.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gnmjscygv.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gznckqwex.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggajwxvpn.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyijsdtq.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gemttrfnh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gvarbesaz.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gstvyenko.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gstyaamky.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gyeawvowr.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gijlfinfb.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gczwijrdr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gdgdjrzwg.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gnbieyeox.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjenppqnx.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gkrejexyo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwotfoig.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gazdeyinm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsdaacbj.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gukbdbtdv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gljewigvi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ghoyzxcac.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdwjytxp.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/giixjubdu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/ginfghfqh.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbkjxjmw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbgpafbu.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gmavexzpb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmbakmrz.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gorjagdhc.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgesorzj.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiqdyxfg.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gcskueacd.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqjnicyd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gusfwmuov.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gslpfzqft.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabghblxb.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glglxeihm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcctppatr.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnvrnnga.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gwsqtjzdw.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gczyiyxfv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gbmdysltr.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gqgvhfklx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gkpxujcth.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/grjnuofrz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gubunkvem.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/ggnzwdirr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gslmqzkfy.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gfckynxuw.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gutugjovf.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkqdxuum.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gctgjfsgn.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwunlnzyz.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/glcstbsfn.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gaztxykyf.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbkjtbgb.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/glglbdyyc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspwdpmhf.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gygsvalpb.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnsciotg.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/glcsvivrj.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/govtdgooo.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsufpsvx.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjzeiczv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyejclae.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxtkkcez.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzedjvru.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgrjingw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfukmzdss.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gpimjtxeg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysjnndyq.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gqdrealtc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gynnscdvl.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/giumtaudc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gojjyfhpn.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjujfulhr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gzzhfdzrz.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjfhjazz.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gdcssxmma.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvnyenlqx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gsscauhcr.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcwdacbv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gdpgpukui.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoqgraxh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/garrgysri.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlbwvfbj.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gzsxnplgy.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gktxhjaau.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxkkrcgr.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/goukfunyv.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfhjaalu.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbjcrqga.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gkraytcfc.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfcamrgr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/givvkwsof.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnpkbgqr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqdpsnmb.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwpewtixi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/grjnjipqg.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbadpwtrq.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunywovab.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gaudbpsax.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhwgsdsz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzajnfrdm.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxlpktqvt.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/giglmzncy.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gzmnewvbt.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqvxmagu.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gypzysaej.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gjqdknixr.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gergwqxrn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzczmrpzd.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbafzqqt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/guvwizzzr.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gqpzftivi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gayxanoxl.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gahtueior.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gqyxphybj.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjwmyesc.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfuxbqzg.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeqwaxnt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpzqoaho.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gkuetxufy.sHtML


<!-- 参考信息 -->