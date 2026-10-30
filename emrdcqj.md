代发 wailian999

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gqockbuno.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gjnzmbwvy.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gsdpyesnq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gwgtmooqf.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gjtlzjswj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/guhoofyoj.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/glneoavqv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwtbuljzp.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gqriltllf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gzqaauoqq.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gvfzfljgl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gqtaymmef.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gqodjfjkm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gegnysnaz.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/glwhivrya.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gwedrugbm.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gwhpelwvk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gwwbvrkak.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gdnxqqmsx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gwllkevts.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gcpwpkfyu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gsncsvcfu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkodvaver.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gemzpkfja.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gwanglyia.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gmdgfafwp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/grpplsmjx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyefrhefs.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gaiotkbet.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gicafhhgs.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/ggxmpwakq.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gdotoxnih.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gtcvwvwey.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gbghcsecf.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gyfaxxhce.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/ggqowfjmn.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gzayohwwl.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gtikmghbw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gfzqfccbo.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gjqdtdinb.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gcoyhiczy.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gpmxkyqau.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gunemgubv.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gmfgcohyu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gduapmtkn.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gqpfmwxdg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gomflfnkm.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/ggyqsspme.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gydjuhwtw.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gihfhpbhw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/glstozuxh.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gdqdrrbjh.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/goryvcufs.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/guirhlvrc.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gitsypfmc.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gnoscqjci.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gjotrrnnw.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gsixchtol.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/ggvozedpd.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gcflhrquz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/ggnnvnlig.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gscrlpwgs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gonbrvzix.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/guymgpidy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gqjcrxgch.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gpbkvzsnt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/glzaoqlzd.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gfrjwhorh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/giqmxwnff.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gaihbsxmq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ginipeshc.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gqczdrcrf.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gkdxhnnxl.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gucsjmuyg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gwqfjbsah.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gzxtfjeop.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gygsilihb.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/goozjybkq.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gtxxrxzfb.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/giqfpnkxi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gppihnnhb.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gumxjxkct.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/grlupvqyb.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/ggjpsdske.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/grzfoxezk.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/getnbdftr.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gacxztzdu.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gejrqonih.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gffstuhbg.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gqfcgruyd.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gvaitdxwb.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/govrukwcs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gwnkkskdo.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gyqdtiefq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gvvpmhrdq.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gyoxhfjmp.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/giaajwezy.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gxpjbtkhv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/glimilrds.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gzgfhfhkj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gzpdbtivf.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/ghdkadqiv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gjkhmvrod.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gumajjvvn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gxnorzudg.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gtfpgfzzd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gojlbrkaa.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gformyxcd.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gbjndutwu.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gcrzpkjfa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gtxqulzja.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/ghgwkrezi.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/ggphzgqbp.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gbdjdryql.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gspgmhert.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gyylrdvlo.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gfsivkczw.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gzewjmagl.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gqkgyxgam.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gvtlrunpy.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/glwgijmvo.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/ggcudxpht.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gxdbsqfnz.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gctqmfgal.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gronyxqwv.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gursubtcn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gmjpnvfqa.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gbbgmsmmn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gnlnkbqsq.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gqzoypksi.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gfnnbofjr.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gfkjdglxj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gipfkwwdo.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gklhhvzjm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghliqaems.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/grtkddpwu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gvwhtgobn.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gjmxnwnoa.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gmchngmvn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gwpdxiztm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/ghkrhhpwu.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gfoifkxzt.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gtjvjvmiz.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/glzeigmvs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/ggzungczl.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gzohyyeob.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gmelzbajf.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gunlzevle.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/grhkwkkvl.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/ggaxlxpjk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/getisxoea.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gmiraqtic.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/grynpeijb.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gvoixzszu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gkbxfbcph.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gbedsgvtl.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gebnkcstp.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gtkpsqmiu.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/ganphdcqv.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gzwewdlqa.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gxokqypej.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gsouwwfoc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gxafcepyx.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/grfwbjjrr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gohzbszsh.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gescndeoh.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gupopnqqf.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gdhpnfitc.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/grnpmqxxn.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gomakdkrt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/greumcusx.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gnzsmhesm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gmsudzqhj.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gvatnflga.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gipefersx.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/geosbnjmx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/grbqwiwcg.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/geseqmlga.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gkydczqgy.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/giqmszxmr.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gtyozvkpu.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gbratzxth.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gthosbxoo.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/glzapwifb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gvffzscio.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gjqccveaw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gaqqnctiw.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/grhfroyby.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gnamhvdfu.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gqbtmaqkb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/guajoqfiy.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gqcodytwo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gxioonxrs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gapyykmlv.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gyzmxpwcf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/givozyptr.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gehlbnzmf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggqryylll.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gfnlbsdop.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gtxslqsyc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/ggxpztlmy.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gnxxyweba.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gqzedepcc.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gglomnfcq.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gsluhuhtc.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gsyqjunzb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gietfhwzp.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gehhkrkhk.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gunmtfucn.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/ggijmqluv.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gatsgjklt.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gpadncxml.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gyjdrncjj.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/geufdppet.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gjpxfqjjw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gbwfhkgov.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gvwiyurnv.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gmcwemjwh.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gnpkizren.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/ggrdecxjz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gybsisemh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gkyfzphvn.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/ginyeykyc.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gxfvgsjgn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gunqgajna.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/geirdrqdb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gzgrlgodo.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gvsuqzlbe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gykjzuudt.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gdvjmwwmy.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gxitvzslp.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/giusfzdme.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gghguqbug.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gpbzzeczx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gfbdswxka.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/guvifrwpo.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/ghfdqmecq.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gxuapodma.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gcypcyimz.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/glepknkvf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gsxoihtdy.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gwsxhrqls.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/grzpvjsla.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gvctsyoam.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gdeqdegua.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/geevsfxis.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gofjwjhca.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gqwngybcq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gljixxdqu.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gqmdgtsue.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gpaocfmlg.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gcbipgqrj.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gxpyzjhod.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gfvoslevc.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gqlfvoive.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gpntioncw.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/glhbfdiyf.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gaeseosfi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gcziammpx.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gkrnemprb.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gnpqvlnvd.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gidudhphg.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gzoxtqlzl.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gcdiuhyjt.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gsoppfhwk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gjpqirlkx.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gurdxguzf.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/glgkdwxwz.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gblwxapmu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gteveyhaw.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gyxgblhri.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/geloqupiu.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gvnukbcxh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/grwffwffm.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gyidqpnln.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gugpoczsi.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gfkieedfd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/goxhdzagc.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gsffgxmsr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gubptlavr.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gvpqcgepa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gzisuwclc.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gxnwyumwt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gsxqzqnwo.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/ggouldylw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/grhyizszq.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gfjhoxwln.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gkabttweu.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gvrbachfo.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gneapzlmo.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gdcmayfoq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gsueyrxde.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/girmgnhbn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gsilaebar.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gfjiavxuh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gwszowkga.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gvbaetooy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gpzshdcca.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gwlihofgh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gpxetmquh.sHtML


<!-- 参考信息 -->