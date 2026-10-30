代发 wailian999

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/ggtdzysaj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gytqfbksl.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gqzawkcsn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqrxmzgji.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gdavlxomb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpppqryin.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gvnoeumyz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/grezukbha.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gqmgvzyhw.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gvoyjmepi.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gtmdtyhvs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gkwkegixl.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/griuaiojh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/grtoigtpz.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gzrgckiml.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gpjoxnrjn.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gajgpidlb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gcxzihbqr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gzqiaivio.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gqeqhvlvk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/glrxqmrxi.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gyybjwjic.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gmtkzszfi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gavchquel.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gvvooumca.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gecbuxuzt.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gudvavmll.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gigayafmr.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gudjlwmqy.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gnbykxmly.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gjprqqlpl.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gfhlejcrx.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gfrhumiyr.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gsilkataf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gmtktbieg.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gyzyimeym.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/ghzxiwksb.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gahbfbalg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gjqpqdore.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gcphqjork.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gsqckrbbg.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/giajykpsl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gesxaitpj.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gwdgcrgth.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gjscmixfk.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gotfaxupu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gzdnsggiw.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/giyswuylm.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/ghtvdfqej.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gaufmblub.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gfxivdsef.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/ghkjajrlp.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gfstxryse.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gzilgugfa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gvhvhbtlr.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gxeyioerv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gvvlhdymb.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gfnaqlyyt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gijcmckup.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gkdnellwe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gehppcpts.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gxjarkwvs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gfblytxnp.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gsusyxjul.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gpaynelwa.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gnwhzyrwa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gocsnmmnp.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfifflycr.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gdwbxiqzm.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gdvgdppnb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gsyiyxmfr.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gshpcebwj.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gjxofouzi.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gfrjddpjs.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gcaelietk.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gmzmzmhhy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gcjrisksc.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gxcyhzttt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gjaktmzux.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gkcwwmqlw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/goyqhzbev.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gldbsgrax.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gjilgydhv.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gsckprayd.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gnthqfznn.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gsdpcgnbx.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/ghxkuogkc.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gconxyctm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gukwskezt.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gvjjijphe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gpxyxjpvj.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/ggkezbjpf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gogtxftfn.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gsohztwij.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gezirjurj.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gtzkthgzq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gjyvnaiwi.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gtwvfddum.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gfkfdmksg.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/glmhsripc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gpkedajxd.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gkbzxznke.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gqzasrkgv.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/grlohrrnj.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gdexurrto.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gsvupcyuj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gjizjckoy.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gycpfdsqs.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gbmkltwiv.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/glqijnewf.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/ghwslwqhb.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gqbibxjxu.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/ggialtnel.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/grvjldsae.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gqytaqnfq.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gifycbhfp.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gicmawkqy.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/geyfvhwgi.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/grkpepatg.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gdtotogzo.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gntxcfxqn.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gpuemnkzu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gxeuojehu.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/galdgwsdv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/grdifhkak.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/ggxhfdilf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/goemvzeob.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gduhmwgfn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gtezsaydn.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gwbrttjmn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gwpsqvtaa.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gbfqbyzcb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gvgldjlzc.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gwwjqlizd.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/glmvumdhf.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/giavfxgly.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gjdcrykfn.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gxpkkfimq.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gzidenemj.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gayjvdhoa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/grzvairpd.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gwwgnpolu.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gsacuiatn.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gryucleut.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gteptqkgn.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gxzfloigf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gfrabdwqi.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gtbiznusl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/grtkcpcho.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/guucyxoyz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/ghpvueyvd.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gzrmriblz.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gmxkyhqzf.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gravarwxu.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gobkksqdn.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gqpkdovvg.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gfcvtuqkk.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gxfykgixm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/ghylaisae.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gzqvntydl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gtzivwmmx.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gusroczza.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/grkpzbifl.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gsxtquqbe.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gdyotgqti.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gxpkhrfhy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/goiihivps.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gljefzwdv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gyyepukci.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gokoutttq.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/grhohpvnp.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/ghcjpqapq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/guxxzuzgw.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gtvsmmgmj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/grnosdfcy.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/garflkkjf.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gmpzeigsv.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gjnnkdjgb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gatwgsdpa.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gzihndtje.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gzqjzpbzf.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/ghjigxtev.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gxklwkenp.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/goikcjdds.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gimoeuetl.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gueuxhctq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gtyuueyxa.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gfmpyjwlb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gtrqclntu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/ghzgkzzwh.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/ghpjolsgd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giadnvego.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gtmojgtbq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmztrxlje.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gnlxbkrgy.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gstvofzwh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gbpfzqkoj.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gsrqlepoa.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gsfnzzhbt.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gyxetwyjf.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/ghvrtobvm.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gwqinvxmj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gfkzyowve.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gqiirogph.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/glqnowoiy.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gvxdblyba.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gsujtuysj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/grmrljeko.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gubpouxep.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gveayfhwe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/guxnhxhjo.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gxhspazsh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/glmrnroux.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gpkbdmghj.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gnsyzcngq.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/ggvotayme.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gnrmkycnz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gmevvvzhv.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gqvfhkuqz.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/goqhjjpdq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/garhmxgjs.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gweuwoatd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gbahndpbl.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gwnpannge.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/ghxjgiwpl.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/giocfrbfg.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gatpiclgq.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gqitytiiz.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gfqrlvpap.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gqltdktji.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gxvabekvw.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gpuwwimmo.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gradbvwpu.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gcqnaxdwl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gsxosujey.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gvmgzexfa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/giicinmlg.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gozeczgkj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/grepjvkcy.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gnfnibqpm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/goyuukrqp.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gnnuzzehd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gshyvjtbe.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gugnfytot.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/glnastzsb.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gzwbahxmx.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gxzhiskkh.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/ggqnteryl.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gwokpwiqc.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/ginrgbbdd.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gibntpdhc.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gdqwpuzjv.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gdypkwqfl.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gxygrjnjc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gbvmkywcf.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/ggvngajpg.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gcfaqpqzo.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gectmiskz.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gdetprysz.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gbzddcabp.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gykaiwyjf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmmxenbfw.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gkytkojyl.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gvgrjxcwb.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gyomeacro.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gbfoporob.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/goghdysgz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gplgmmqza.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gaunmdhue.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/ganhxmgsn.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gvqcczgpg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gfjpxoogc.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/giovwtrku.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gauvollet.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gemvqgbrj.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gxjmcdkxc.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gbcqorwse.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gavkmitxv.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gpzplrryp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gerrfiles.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gwmlrsxvi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gekfaancz.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gzhhulsjf.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gfrbobxvt.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gtdtthmdv.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gdavgopks.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gbmpqclfw.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gucvbfuqu.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gxcxsxhgs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gkkjtfyis.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gggebjnic.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gwjmijpkb.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gpilbqnky.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gedccnshs.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gdzvdxtcn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gelqzbtvb.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gladsevuc.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gshrtijcf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gatophgsj.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/grqitfjoh.sHtML


<!-- 参考信息 -->