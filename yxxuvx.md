代发 wailian999

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2fjdckxcc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2qyvvenpq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2savzhlaz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2dhbrrkve.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2brkfiwdg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2xnftqctl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2czakioge.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2lvpxufvl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2hcayccvy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2gdypqrie.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ertzwdli.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2brbepydf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xhavoarb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2dtectnnl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2idzapjax.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2afqhhdmo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2qpoppsnv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2kocegdsi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2rygkwhza.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2vezcjzuh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jhqowlvc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2wymqsklh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ynumfokl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2hskkgcpx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2kibwldje.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2batbjjao.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cmnxahis.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2axpmxyii.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2uohiydnj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ptkzfjjb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2lwybebzj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mulicpat.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ghramyvf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2sxkbeclw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xcukjgnm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2eclnffjd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2hhwhijsh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vefxxhqz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2guvumeil.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qzlheecs.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ahthwzkm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ohbrdeyz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uqbowajg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tmyrdmci.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2rrjchalf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jbokpmji.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2uoujoemk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2vismwdeh.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ccitcjet.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xwiehgtc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2cxycihfs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2tamprlvn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ntadqfnx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2aozgicxo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ggsmrkrr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tvfmlhgq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2wzeuinbw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2uxojdmwy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ouovmdic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbnwuhqh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ddavvxsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcucvbqm.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2khmjcbju.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2rrvbjdnd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zdrmsenw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2skwbjjnq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2infbdebb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2czjdxiav.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2cvcjstjv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ffegksdy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2twjglvui.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2hypfpqnx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2qfqaujhc.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tfyuhase.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gzefnocn.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2jtttjmbi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tnphxnln.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wugdasdb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2whwyxnpy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cgntmxyi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zxscmtvs.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hknafygd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2otdbhqqf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2wxqbmzjf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2kjfbynlx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2zaiinfjh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ivzcvoue.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2mzxzzhry.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ssnrdpmw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2opdfnody.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2radkizri.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2iyiubjyw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tzetpahs.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2psecgfeb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vhgmhlcu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2myaxtddq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2pdhuumlu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2wvdphssb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pgkihidz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2trjjwiym.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2amqjvfbo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2zxbwrvuf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sgfntneb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jssrnigq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ygilenyr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2alkyvbwo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xfxtxdbu.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bcfmqxtb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2uzgieonu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xrrlwowk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2fghenypm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2oyjoxfyn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2mmjidbny.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zjzghsut.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jrnbheih.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ozjhrqax.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ulaepjpx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2azhetwbx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2cycvolnc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2vknxrbfa.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2afmxadhz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2cddvaoru.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2mzgflbhz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wkgjeuhz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xckwujda.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xgjmrizf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2procsnlb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2afampisr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2efpsnvlh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2vyvatotu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gtfaohzg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2wtzslstv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qphpzywk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2nkwpqhfo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2nxqapqrq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2nmteawen.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2lvgclifk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2cxgdkqla.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vdgvfico.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2qpngkpho.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2genrqzwy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2jxphmreu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2arxcvzpq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2wsevjelt.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vlqpuxtu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2rfmewlht.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qqbxgsmq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2kpwklzxs.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qyxurwjm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2hwdcirtd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2bjtynsqr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2teennpzn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xdqdgrmp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2iwqxclka.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hdkcjvfd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2fsidpbyw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2merefbmj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2dggrlojd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2owtlagzf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2npnhssna.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2emuzqwlf.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2zhqhgovx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jceuncld.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2tkbotntq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ggixzaae.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vuncnyux.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lryrsnpv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2bsgkcqwf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2efcdnmjy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ngqfqlji.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zcadtcvf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wnyfbddj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2igvtpwuz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2niqjmelq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hgxxkebc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2imdanpkj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2izzvqipb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wrayvgnf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2lhcsbxqs.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ywkambgu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2uprmdgoc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2owputtaw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2bxansumm.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dpjwbmts.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2dnljgtoa.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bjduvvfg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2tdwatcri.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2cjtjegld.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2krsidttl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2mqqadfia.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ithpiuwe.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2hlozfrqo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2orxulaxq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2jpdqfayi.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2gpdxrujx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2shpqzski.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2okglbfrg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qunftsvr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ndyiygoi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2jeamelho.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2vicjkoiy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2mlvtzrkn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cnwwijdp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2mntlzppd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2liowzfrs.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2asnysqqi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2tyfqbrja.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2huwmwvwu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2pedpdrej.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2gyzrjvyb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qiqegrnn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2qubzewyi.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2pzbvfgeu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2oiuihzus.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2mydjicqw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yuodunhn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2jpbtudui.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ycmyyost.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vreadrtn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2reaqavvg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2uayfrqdr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2duowulna.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2rtpjtkjs.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2cgsvetgh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2dbcvtaew.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2dztftndn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2yictjnwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcsalghf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2fywkavvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffbolvoh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ktveivbu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2xvpknqwh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2eidimjvv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2sgltolzw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2nhylofhh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2kipuhnzx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ssdroamw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ocgaxyqc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rrcvyvhm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zvogomyl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2odrrgcti.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2reaejpla.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2injsicsm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2efrfxrga.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2wqhlnjjg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2psppvdob.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ktpsnioc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rdgfkbeq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2upspdqvi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2tlvxmzrf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jomcxkgs.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pxxjqoth.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2xbzzzjmw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qxcwnrzy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xtuzahmz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vtlwvgkq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zsbwvgjr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2umpivzvq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2gofnahon.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lhlkbsdi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ccapnvcv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2esnifozr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2bxwhwmxt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2kbdhivup.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tbdnquxz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rvcgynvg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qdewagqm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nkfhqiyb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2plbruzzn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2cbudgbca.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kyoqiebl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2hepzaqdu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2isgzqdyj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2apxzdmzw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2gsxftdgi.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2svtrfozw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2oqvudbfe.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2xeavdtsa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2snuzwfxf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2hmaokqqy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2yuwccail.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ykvdbwcd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wglxaptq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ssiudijj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vzvjzlzs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ooroxhty.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wqcvyqhq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2litsnjoq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2omvgsmbj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ooqnqmao.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2jnfmpjzm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vqmqjiqf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2micupbis.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zmbrnbhu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2pbadiyas.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bexkdjxk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ktaxyaiw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2lsnighhp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mxmqstss.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jtyajjrh.html


<!-- 参考信息 -->