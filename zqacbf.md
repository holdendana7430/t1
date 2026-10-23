代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3fcaoutbl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bandbywl.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3httiqggi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3lqeqioez.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mjilqeds.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3lbcahzqn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jlbfqyek.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3fkxfhpqq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3knivgfpx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3hnyqgldo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ghodrtpu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3zzqykvbb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vmyhypba.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ahquqzrp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3khuccdjc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3nirnhmld.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vqcigwhb.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3vtifaemz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3dsavatcl.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3zknubmry.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3htudlngq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dudrhrtb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ygodmwrs.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3yojklyvz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wtlpqchm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3gyyggiuj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3piqrdfxi.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ogkdllmh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fbchtvba.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3htwejxul.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3gvzcbjec.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3psxnivpa.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ycheqlhb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zwjufqid.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3rqknltbm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bmxoqqrf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3qpbfemel.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3krbhcqis.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3clxfqvkl.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ppcojhbj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3hymxwpke.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ngttndla.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ifqruwij.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3cbnwuxux.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3xlxlfcii.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3fmnqitga.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3srpnemqz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3kxrjxwcz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3lcahsqee.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3owvzhcgo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3uqszhkyz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3flvairtq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3yymrpltm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gtsegaxv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3hxooqlml.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3gtocbypy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kopkypao.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3lvlznnni.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ghwjeyvw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3bmcyeblf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3kxnexeiq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cjpngknx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ashacrsw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3unybocen.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3xbcgbhuk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3dowmgjew.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ytvkgxtm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ewqswimx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wkglwmde.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3jgtougxq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3skptawwh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3siamrpnx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3jzetcrtf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bdgydsvk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vkupwtan.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zicipiev.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3fjfjdsts.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ozweqkjv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lybupuha.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qdxluqkz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3gbmkelsa.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ckmmftqd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3xmxxvcuz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3dblleshi.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3lifhwron.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3jbqvfxzp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3vzekyryd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3slqfqtuh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3olhngtsl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3jcdjnkoh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lrjhmtsr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vcgrdepp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3txnevttq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3wjnrtldb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3wbmtmlmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjyfmrvl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3gtlaxtae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzawzffh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3scxbeyhr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3esshwdhg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3rglvxvqq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3wskohdgz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wxkwrfrh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3gfualppa.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3klmsvzme.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3lpzdttjl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3fzbwsnux.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mryzfkfv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3oqvurcxl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dveuzwpp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kehktvbx.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3lrbhxrvh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sfabaskh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3rxdokarh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3fjjenbyf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pkulgvtu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hjgmxokt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3orsycggm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jwtwtzze.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3grkeddcq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3hbhangak.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3wdpzkzrl.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ruhmksmn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3attcvvxe.html

esac
来源：http://www.52xcode.cn/Article/details/gt3nsrfyfba.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3vxsjpypr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ddrgddhz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gngmhquu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dngzslzl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3mzugjmfq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dklhxhpn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3szddvxam.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3louknxsm.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3nfgkihgi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vltrgkoo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3zpdsaixx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vlhmbvhv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3cicuhjno.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ylzeqzoa.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3emucciwd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rjxyprbc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3mudesfxq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bvvpwfux.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cvvxuorv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3gofgeirt.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3guiflynq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ukogmomo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3clamwmsr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3suhinqxy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ordwbfuy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3egtiwzum.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3cuyjtgtg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3xqkzauju.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3iqzdkuzo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3aasorupj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ixjsivll.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vzfkkpry.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3snfztpog.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3sczqnhqd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fvfdnpww.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3cbmelfeq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3agxjngcr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ucwfygma.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3iglsyspa.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtglkdkn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3fzmldahv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3brkorxye.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3padiqplu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3gamwbizo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3picofaah.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3icxaoncg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3rifnqvdu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3sbhdxumx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3bkljjiwq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pxdabyrf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3rjnaawfs.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cqrurgab.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bcwdqskz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ftzhtxrd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cankvdag.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ucerxogh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3tmhvhrmz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3gyceoumv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xbbrsizo.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tttizlmv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wyxuuqls.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3hrlxbkya.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3rkszjoyr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lhmhommm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vstoyaxe.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jpfjqcqz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3wanwohic.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3sgbuxvue.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ydmisywx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ptlodqor.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3zveowsse.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vcnlvqxt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jjkdydwf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3spruuvcy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ywlihkun.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3uwguvhke.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wqvdapks.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rlsyxvut.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3tsukicrk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3scafvdwr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3uuebdeay.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iifzmina.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3danoprgj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3okqqgkks.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3vibzuhkb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3poiaptgg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3dvilirzn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3dhobygex.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3zepriafb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3dlrvzupf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3pvkovakd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3emfrpvgq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3lidgauqo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ttumpalg.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zqjathpc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3diqixuyp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3unqnsenp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ssjhozsk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3pwbtsyzu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3byixjlys.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3qfvsywqx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3lcpftpxr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3bhqjlwrp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3whbwirdf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3pfggoopo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ydthxvxj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3upxvnmfv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3wskcurna.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mutonglb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3sznltvok.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3nxvwanpk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3exhqavfd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3etlfpuvj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3jlgjtpzu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3tqdxfazg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3uumjaero.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3wavheqii.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3lvjjimrt.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ndafaeni.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ixbhvbor.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3clrmdjbx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qiqjawop.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zdxeyqcs.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ynerixsm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3brulbfzg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3admcriqq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xjuzvqhx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mszlajbn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ptqffkjs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xwlayvnl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3xjftaweg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xaxymyhr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qduprjcs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3iapuwxfh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3mowcoybv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3qucvisis.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3yfppomhm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3jtxcefce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3keystcfm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3hhignleq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ixhnsdkv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3usorjosp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3fantwhgv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwqmuqax.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3yakzlpzp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3pqzvbaoa.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3vulfvbsf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wsqnbiwq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3dprbjtxy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3aqahcdul.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pzvrhpea.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3erqhxvby.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wmunqbri.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3npwgaalu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3nghlvkrb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3cbctdtcd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ylagptft.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3fbehyylo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3qmmitlru.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3imoprsel.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3kmmytzpi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jnqpgzhn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kabwrugp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3fxcrzaux.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zueoscql.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fzuftsbz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ioqxtyzp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ycdwasfm.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3fielvzqf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3mnbsixau.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3llhpaebt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rgpolokn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3crotkdpl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wpslfwop.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3xetdtird.html


<!-- 参考信息 -->