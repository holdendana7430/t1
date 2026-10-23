代发 wailian999

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3dxtwkbzi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jtlsekil.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3afwazrxf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3yvmuvhia.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3pemxtzkg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jpadrzma.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3detnbfcz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3bneahxpo.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3jbwozzuw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3codbxdwp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3fwigeuhz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3nxzokiig.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3phrvttik.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3foaagzxm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3edfzuxpi.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ozhwmysb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3gddhbsdh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3vyfotgsf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3dycwwben.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ivaivxuq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rjobrhdg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ljicqpzn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3xobyojlv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ffsufwox.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3pasxemkh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rvwdavlx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ctyghzme.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3abnahlrd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3lvgmjdyb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3zhfzqscj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ospdyazi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3zpshvahg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fyktlhvy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ozodelpc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3afzpwmld.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3azteogkq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3bqckqdui.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pnsvjrcj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cmytvabp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gfihvoov.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3akypkxyo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dgnvbdqw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zyownzow.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wlniwdmb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3lzrmqlwa.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3shrzksjc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3klvdbhxa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3eneztsfi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ywelhpvu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3wlqcowvv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3opzxnlpy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3kcwvbozt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ikbvhicd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3zvymdavg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ljugkmkt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3goyjmkmy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3mqgzgycl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xfywikfz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3wucqfksn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylcmtddh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3kwthiwve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hfosyphz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3mrnnrpmi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ukycxbkc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3drxvcybl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3kfbcyodi.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3mestbdzl.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3afcqvhrs.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ptypskvx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3aodsljst.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ehtlozks.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jkkecdoz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3yblamtzp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bsjazcjl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcjmqrmb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3hdxobrrv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aupxpylz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ctkxihez.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3cyqkdmoo.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kzipzfur.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3fpkidoux.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3dezgisea.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3njibfzwr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3fbbdnajz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3unqgozks.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xeiaqyts.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fvolxnon.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3nzmpegql.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3pfauehod.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3tiwpsszn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ljgfrldq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3pszalpww.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nppiswqi.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3gpubiadr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fkjvrbvv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dbdkpuzb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uqbdreuw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3wsaupofa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ojoepgvz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ybvyoejr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ywuyjmty.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ircjowdg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3tfjidnns.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3sxrrqjpp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3srazcfgc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qxycyfgg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fbpqccqt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hxxstdfg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ajcfzbqb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xoqyjzfx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3crqgqkuh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rranqaxb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3rzzhhbsa.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ywiscxiw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ofqnzmik.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3eslpwsad.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3iaollvzo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qunjkkjc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3fpofyjpm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3uywpslbo.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3eqmbhekf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3yfskzhzl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gzagrkqb.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fzhifkmr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3zgivpjni.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uvisdtkd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3btcfvwaa.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3gktehmrw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fohkwypm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3pdwiqsxo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jgfhjtqe.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ihlofrsw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3idzlvfiu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3pgurhomk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dwnonyqa.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3naymxxzm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3qyjeayza.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3eafennvf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3iedrgfvu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3smxndgxj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zrevjrnj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wkwrihmi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wijgmjnu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3waqlugyy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mgmbzznj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3jwqxalwv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ebzvmubf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3fzrkebea.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dmffaror.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3xeanjbyj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ekdjddxz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qszurzje.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dhmakygk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fxtkjjos.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yyxvpdmq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3mhpasrtr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3vskxekax.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3fnyxvgqf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ctadchsk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3csmrhcpn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ngqnpuzq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3tbyxfeew.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gpzupupc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3jdpughdy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3arwdyfxy.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3oajavlhy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xekdwwoz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3nkuidbwd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3cdaxgjpk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wcmhxwol.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3efmdxsxa.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3harvmydz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3bvxgktut.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3bzaraqki.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3eymskpxd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3eldqtfkh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zmdpsbwy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3owmesfqd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3smpswumt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3jviahkth.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3abcjqfcp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ssnwmhof.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3bkkkcuzx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hvsvsmmw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3qmaswmdf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jbuwwnxp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3cxrytvrm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3bsemaynh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3rnbmbjhs.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3etnqzkgi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3gggqfhel.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3kpybdiff.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ujotmdbv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3duarqime.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ulqxwwqz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ydemuswt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3npksnuaj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pqzcrpbr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3tozbxbvp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3knpddxkj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3stgfvstq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ibyvlxet.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kmxnrqsy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3latazpvj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3nqgncuml.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3lnyruata.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3bvtjdolj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ikpnsnhs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3azkuybus.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3nbwjnrrv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bssrqyop.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3fcrwvaqb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3xuzcqcoj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3glgfebxg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3msxzrvyo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jibmvqje.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3vmfqduun.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3etnjzohz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fclljwsc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3qvxxqjlq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3zwaercfk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3npjvihab.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3rdithhwk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3nqyfyrmw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3agflqnfo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3lvuzsxhk.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3chkhpois.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glunhkqs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vmnnkyck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hsogtusv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wgmxtrwp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3utankisf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3edcbfrwo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3dtgdzyic.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3lcoqribs.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wrpjhhak.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3fodydsii.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ncqvrxij.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lqmwqcqv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hrphjxkz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ofekxbca.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3afcvvkty.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3oebqhbmr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3gjafezim.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3sylufebn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ofjhfjgo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3lvbqbphw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3tezyuchx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3okfdacwm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gpgghgpd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3wkyjanin.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xoiqjcol.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ittclfiw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zpsqxflq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rfkfvwck.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3qwofbacr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rjndhewh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3adixmgah.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3spjwejoe.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3yscdwdhj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3dkfoenfs.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hqoknoyl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3yyadxytv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3gbjzsmpm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3pqslwajn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zsghemdn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3zejkthxh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ivnesuia.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3upxfzukn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3qqkejvyx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bhlmoewp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ywiwtxrp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3aenuppae.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3txmlkyao.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3wfzbsxmg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ziphswxn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3pijedejv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ngviqptv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hnjmjajy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3uaeagzub.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3maqeexgr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cgbwsjfw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nxwfvjnq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3sqgdgutx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3vansjyjh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3kqjsdjjd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zevedgcc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ruehuksv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3azzzfpol.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3apignlkq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3gwflmwxy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3jswohxfd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3fwzbvpiw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vjermeeu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3uebryxvn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hgkbxeea.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ckhfgypt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3kyjpngms.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oqhisvyh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mkwtflwy.html


<!-- 参考信息 -->