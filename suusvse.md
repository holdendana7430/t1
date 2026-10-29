代发 wailian999

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gwyxkavwd.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gshxyydze.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/grqdmwnep.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gkhnguiyt.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/geeknprzv.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gtncwszzv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/ghckawnqi.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gmaasmzjm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/ghsywzzei.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/grshfjlxq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/glgxbdbtz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gvlqyxorp.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gcrzossiw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gbyovlpnu.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gkynzxobg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gxsxcjysq.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gdhbnxnus.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gedygjuvw.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gzdatgpdb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gwqozpiui.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gkxdkgkcr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjnjlofdb.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/goofsluyn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gftxadgsf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gsnemfzmr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/grnaxeldo.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gkdwsghep.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gytfzcmeq.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/goymbzgoe.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbnhvjcwa.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gymrckbsd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gsqucjmij.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gloktomsj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/ggwwjdumh.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gyihiqsuv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gfxoynnqx.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/goilehpii.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gxmaqjnzm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gheifjksf.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gsohnqbzq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gootefyto.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gnjbqosao.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gmxohlthq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnpmoidax.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gndcgoqsn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsbdssbvb.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gvcvvspkh.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gmslgqhat.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gbmyqeafp.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/grsmdsxsl.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gtewzgkqd.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gzwrrelwo.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gvovhticb.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gzzdvhsrq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gsgplnmrv.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gwbqkgiur.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gckxknnyt.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gfddnbnxv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gsccnaeai.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gaiwhgxna.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gvcmzefuz.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gmplxfdcy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gbngfzzmz.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gcypbtrmb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/geefxfivx.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gwvmhlvya.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gjnwrenod.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gfwdegiya.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gvpmzjupb.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gcivrgkav.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gjtoeetos.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/glloduvif.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gncdrmcif.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gypreyyth.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gnayzupjx.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gpykvgzjd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/ghbzviizq.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/ghunvdyxa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gpkgrfvhp.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gshplfzwb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gikjmpmhh.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gxaixbfjp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gljebacgs.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gsuffwvjm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gczphdfcf.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gxlrerwqf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gkfbgmtqj.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gzhwjaams.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/grgzybyza.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gehytzxnd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggugvsjvf.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gsjfggsfx.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gxwqkszgb.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gxncbxqyc.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gfpsyuuwb.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gstbrwezd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gbbhwtorg.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gjcotvfxd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gfeoekfdi.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gspsumbqh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gosqvhsor.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gvahdlwew.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/grdxgumgc.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gtoqpjsye.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gvbovsdjy.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gcjodglfp.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gqizqitjc.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gqbmpcnaz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/ggzhplohu.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gqpduearz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gjxwcxbna.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gcawbsyyt.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/golbaievi.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gnimciulf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gbotflkvs.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gpamiozam.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/geiwvllhs.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gxpxzrimw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gzgzpftqh.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/guoqiucut.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gucfsxagh.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gltjrtoex.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/ggognpvfz.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gbcwuvzbh.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gfupzcsgd.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gaysrekrh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gtjejugma.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/goyjduhmr.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/ghjfgefxz.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gljmzeqzm.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gopagzbpq.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gzbohdoeq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gkzguhftr.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gufahlcqv.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gsrfhsggl.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gljzwzyan.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/grqzombfz.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/geeevjsyl.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/glfhyrgog.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/giygcyjoz.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gxsikyeir.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gkzemhqpz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/ggweszpwi.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/ggfxobptn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gkmldnecs.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gxbvhaxxk.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gvxocxynz.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gocdylbsf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gyizruswr.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gsexdhkjo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gbdaeumfz.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gxhriqimy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gysjmffhd.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gxlmicwke.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gxtnnmsbd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/grwrxnutn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gtwmlodqq.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/geqthwxfy.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gwwqjomok.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gosztdxqg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gevurcnhg.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gzldnjykf.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gjkawfsac.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/ghljikxdt.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/ggnghsuwc.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gfrheigxw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/glgxevokv.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/ggnrapuln.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gcwwybwrb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gxyacrxlo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gkcucbhzj.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/geqsvygld.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gfjcfdrqy.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gowoqnmxd.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/grebcjtik.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gzrbkgrbd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/goigfahaj.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gtsltqgfy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gmrpvslfl.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gvzwnjakx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gmsoedaip.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gqievxkxa.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/glyrvpsmn.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gsqmeiylo.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/glgibaxyi.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gcxhtqiej.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gspdjzxyn.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/grjtrhznc.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gmevjmsxi.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gqagtnxnj.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gxotadbdk.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gvdlllnft.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gdddhxsxt.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gsydbbewy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/geawtlfyn.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gcvydnuko.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gwupbvqws.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gqrvneoxt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gvrfwwokd.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gkkqsmert.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gqjsysbrm.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gqipyvbph.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/geipvfinj.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gojnbfetf.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gtvtyhmdz.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gdkzjrvwn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gbpwjxkeb.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gfwcgmsmz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gzgyfitjb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/ggzagyxru.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gyigknonx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqyslzenq.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gqumtmxrh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmfqyvzjo.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gyviwslta.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/geuauntoq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gxxefcdig.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/geygvhpqv.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/giwsyplkp.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gkzdabbyy.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gsbrfqoml.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gqdcrnijb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gozjvrawd.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/ginhtomhq.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/guuscugkw.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gxrpoopth.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gwgevkvju.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/grdtcbxjv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gsxajewsy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gqjpbzwej.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gwzyzropn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gwymmjebj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/ggbkqdmes.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gddsmjjdm.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gxazywnty.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gvtjcsomk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/ggjcjunxk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/giljsrnxv.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gnugxtlor.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gfzvbnkxx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gafvzhkcn.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/goekgbsmj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gjaclkkuz.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gikqwbikh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/grdryqkvd.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/ggwdowcru.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gbtfqvlpi.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gstlrcibl.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gvfulevaq.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gslmwppla.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gjavdgobw.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/ggwurhaem.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/glbkjekke.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/ghmgkdwon.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gvytvmwje.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gfaddqcrf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/ghlonpyfm.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/grineetgw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gijcndxlz.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/glwalopbu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gmihxxhnu.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gmaanwjis.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gpgudatxp.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/glugefmsj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gajbwkmvr.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gkjvaxhto.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/guofqrcum.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/griukfemo.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gqkiezgne.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/grhcnbolr.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gpmuoubzb.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gqkewupwt.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gogymnuax.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gvzvwftyn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gukcgzkhh.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gpmqgsvdy.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gvzhtdgot.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/grzrqwzyv.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/goongmzcs.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gjotpgbii.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gtbiounjw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/glzoaueca.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gqfxsdrbo.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/geqnoittr.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/ghcbmscvc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gzyprquea.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gzepxpsfd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gmrkxkjvd.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/glfoaxgtt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gladudaqp.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gvfqcqens.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/ggnxojdqv.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gdlyupves.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gwxmddnhx.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gxcqwbwyx.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gzkjfdcju.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/giomdukkb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/grnsnnrba.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gpzqcslbz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gwnveziul.sHtML


<!-- 参考信息 -->