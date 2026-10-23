代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zkcwrxso.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3lupmhmml.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3guetnwsc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ibmiezfg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3uxlqayvq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3hnspvvtk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qxotzgiz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ywjjmqfo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3eoijfuiw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3exrgrsti.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3htungume.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3juzsoayx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3scqqfegq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ncjovons.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ahxksfzo.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3qmypscoc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vbjfigis.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cfevtznt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kwsbfbfk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3lniiygwv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dydxnjwa.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ychxrjtz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3rxlogffn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vfeoleyd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ijtfvctz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gyrzlhly.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3jgxvhkvz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hgrgorti.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3cobjekfo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3hfcvmhyq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3dakytkvc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3cgdpnmgz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3txnzdevr.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3lgbzuzpf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3owqjmjdg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3uplfjyxo.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3lvtavvck.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3jmcwhcwc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3xvqvtlli.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3hpxtvrbx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3vgwwaydw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3sbzwcazv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3crloeylk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3clckrosm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3rcarokwq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3wlwbgwoi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ucsqrogm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3uejrufcj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kaedqnxt.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3lowqpyxs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3nkenwirg.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3jcpmtkqv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3mfbxjoph.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bwgeowor.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dftlxidb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3bdffthxk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ojkwgdxu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3cypslean.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3kkceqaen.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3vxiosipt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3reddbqgo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3uvimrquy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3lsuqudsr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3cnwshsko.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3yzzlkgcy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hamvyijq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3sfngoamo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3polldjdt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3aewwtmzk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3whdofpdd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lwotqruo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sbzhcqdl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3cifemysx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3glxqmanu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zaobxuln.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jdcxvnea.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3lljwyjmc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3bxwfsiot.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3rasqkixg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ymvorojd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3pjgqaahl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3uhsfgiqo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3raucxgxx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fdjjfzim.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3tntxtltu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3sqwotvbf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3znvvbzvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zpeekmjt.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hxmzrxxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cskfvyvx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3qpstjqys.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3rwaouyfc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3cmuepkto.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3injxlrpp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3fgjvypgj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3wqfusiqe.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3oxrchtqy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ymbxqidn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3moooyjqg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3tztmdjbz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ixkhhygt.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gnsccatd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3djhbnjop.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ozpoieaa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yyvqkwst.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3hkezkdan.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3qxhrbfzc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yeyzpodw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dwmxbbmu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3iizngucf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3arxtvjyn.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3qrzvolgo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3owkuqwvc.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ogtbvsfv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3mhxhwbjz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fzpkhwub.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3bbccafio.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3esnjcfgi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ezrqrbeg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hurlzejy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3egqconyb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3znpqbrli.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3abyxsqph.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ehilxwxq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hdazdvto.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3rdglljgq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vemxrzwk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3umwaupoz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3xfagidif.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jcluxmyb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3udzxrvuk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3djejjoxe.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mrjeimmk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rdotrevo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jystehua.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fuxgjgmr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jjferebh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3grldpyih.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3uvnbmkcb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dyhmdnkp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3bqipsdnt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lzvaxfvf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fmmzrnbn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3grhendqe.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3iehzfuuy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3cbabtgwf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3swpfrsup.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3aazpvjcv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3qjrnipqb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3iptobgfg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3lybwyyed.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vkqpqcsk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3uporrxqk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3vrozhnbo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3fdceqrqb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3lwfzzsth.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfogormz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3puhmgtzw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3blqfnqgq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3elkykoiy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3nplhznke.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ejjawbvb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3yneqcqud.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ryvzrfno.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3uqvvvjyz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3vpvteozl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ynxtyjkg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3xakrsgfx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3muvonmnm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3fikwiugb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3kegetdxj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3avqahhvg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3iwgdiflp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3udnxpdjh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3bkwtvdmf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ifrufqcy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gcgnjaqp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3hbpbqcoa.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3cegpsifo.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ioqrewvo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ppefjduh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3cylllnoz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3uwkaoscc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3cvbbahmo.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3mddsufcz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3dmsubypx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3nytyjyry.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3eauvxrzq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ejvypzsq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3meayifjh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ltgjrsff.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3wdxhywov.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3jwardcde.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3noijrnxc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hhejndlx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3yveelykr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3xhymmpoy.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3xfobnlro.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qlaxzvhm.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3hougkxbg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3xdshzcen.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xaaufefm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ysxntkdt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3jlrxksyb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ddoyzerg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3rzuxesod.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3tikqrroz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3vdfocxhp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3bldslmgm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3amgvaoyj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3nrxgujmk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rkqdwfpz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3irwgadnm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3endvqnqn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xpipejcv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3kflspzgi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3svzvhlyo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3certqptd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3afhtzqdm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3wagrecip.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3gxehxoju.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3joaqobjm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3aqntdvga.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3syfopfcp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3mguseene.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vcprqjdp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3dwlpncmk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ysohbbuw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3sepzwshk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3pyhhwrdy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3eafncphr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3hzwcagxf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3shbhdwos.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3fpyzpgym.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3nlfxwkvr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ixwdalug.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3vozkkqxc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3uipdqcxc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jjsshnzy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3qdruzggh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ppvvievl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3iqpxybik.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3medeknmr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3imfizntx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3wumpounz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vnwgmcpz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vksiuxyf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3fwfawizv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3yoqrkycp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3jfpfuzlb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3rkvxjqfq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3pxtfrsss.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3zkkyaxbs.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3fdfgkzmc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3jgahqnaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrhhoyzd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3piojogxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abenhknz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xldcmzkk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3spsbcrkx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3harpikwt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pqiuopfl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3emenwdvc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3lgtxgwwg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3dsoaarpu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3fwomcrpk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3rdygofox.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wuurdxch.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3mblvofug.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zlvyfhej.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ywkdceso.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3dpxgvbjf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3wzxwmdjv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3wstfucmg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3rwpqahlx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3drahvbwn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3czbvyjxq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3lqpioqhj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3cnvubndi.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3exvdjwfv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ltuxgpwh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3nifniufj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qrwwjhwc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gvcauajw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vtdovsvk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ybpgqdcj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3bmkisnor.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3voawztbn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3kbguinsn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3plxhcvew.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3qqrujwoj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3svufqanv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fzmvtgln.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cxkhustk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ntdoavts.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tvogtzqy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3qheoypsa.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3kiowfsxd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mvmuaexq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3nmqgbhju.html


<!-- 参考信息 -->