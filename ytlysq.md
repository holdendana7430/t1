代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qzmzjzgj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3suptiucj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3zbcpsewd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3okdjqbsy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3afaihfet.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3bhnsgnvw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fcoaltkf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3htpwlwya.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3luyhvfuk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ceiwnfgc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oiqhiwbo.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3sugzngvl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ygqhzson.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3fzsklwaa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ezsweyyg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nztulswt.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3fwnhjorn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cjxoujza.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3cxdddjdi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hemyqhbe.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3rzmzeoni.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3czueowif.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hjubgaop.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3rmvoinao.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3jrjkzkid.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3rawkeebt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ccsddmsv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3nxqxzoyk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3idfbswle.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ggdduenb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3tfapbmha.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lwurktld.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3rvvzzaij.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ovwrlhpf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3tylbndvi.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3xiioijif.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3slfwsxeq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3digabltc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3kxnluvqb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3dgwvrxjg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xgistzsr.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xsprpqqk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vqfalnxv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3okxdrogm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3bmfhykjp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qplpgsrb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tyzzinam.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3xypzsdru.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3wzccxqbm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3itebljra.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3enuezxvc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3vrcshcxr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3obijfzwq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zdwcbbnl.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yuzimwax.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3wcdogchk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3duzdtcqz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kmeaqlhd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gaaponmj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gqytgcim.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jfzfokik.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wuwayjwm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3daezehba.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ujrwcadx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3dzkkwvmt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dbnimtfh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3twukeebz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3zshhcuyu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jqmzjdkd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3smgcfoez.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3vlydybtg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3lfvzbdho.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3memhybuq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3svqjkdmh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hfqrzbxa.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3oobxnpqb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ylyauhny.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3swvrjepl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3bmrfqmlq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xahvurkn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3htxtbzks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3poctgpfe.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3iwdtwslw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3zbtvtkxw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3cxyzdqyb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3egynnfif.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3pjcfjldx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3khqspnnw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3kcqcydhl.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3udfcyytb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3qjfseaqi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3atbtadfm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3aqacavre.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vwbbvlvi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3wahuzltn.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3gnrghiaw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3emtefbdj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3gzaklezv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jhssufiv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kkmvlwcf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ebjkdujh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3curdrdag.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xjxxaorb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ditgqxwo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3itewasku.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3vpsblong.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3tsdlpztu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zldxfaec.html

esac
来源：http://www.52xcode.cn/Article/details/gt3sdrtcvwa.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3neehybep.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3hdvqrkpj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3icjqgvrg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hglsdbxs.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3cohychdp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mvxyiryb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ymgsvanf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3sbtyisow.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3fjnjfehz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hoshizwg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3uefobjpy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3cbdkzpny.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3jqyrxofa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bjxwffjw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3awbtirwz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fibczdks.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3hkyfkjhj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3snnfwbro.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bnuxguvh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ghescnlt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rkcboqcd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3chsvfxdw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nhpfmtbz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3mzifmiid.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3egmkxseu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tgkjrmkt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3mdvohuzd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3pppsemnn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3cyracfdy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3voiczlew.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ylzlgtmk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3elqcmjyl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3gkngwiwl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3nqadvbem.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3swdmkmoi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3spxnxgok.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3llcefwph.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qctzxlfh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jrrtreyu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vuvjbyoh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qmyenknt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvweaijp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3boxprxdm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ccqvxnzm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3zlevtlfj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mpgtomnk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ftreznay.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3yzfhfceh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3fdcvajay.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3fqawvfxa.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3lkajxtqs.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3jfsilobh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3amzrposb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wclknrne.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3uzuluofw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3irjoqmye.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3mjblejcx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3mpyuptbs.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wvwsgpha.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qjvnbzam.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3stamufco.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lbdgulkg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3skottkcv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jjjgyjze.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3qfzhxjjg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3joftkbkn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3tymqawsy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3zsbnntul.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ywykkmnw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3edsszboa.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3xmdkfhrd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3axnwutii.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3sgxhycup.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tsfnqhad.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3otodrakx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hnumbzab.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3aepzhhks.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ymsbnvgh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3khusypnp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3tgdywufv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3dttbwbci.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iwdvgmtl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ixclmanv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qdofcpey.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3rntorgwv.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xjinoviq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ylhzjvdr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3sntvcxwh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ghlcczlg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3lhobactm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3wltexshp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3yshdrnkj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tuekeilo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3aygfmlbq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ijaccgou.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3slseztny.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lwztpnil.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zolvkoia.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3wjqkdhps.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3uafqazwc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3yyazyeiw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3lwbespfb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hdjsknuu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3tpqjtusi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zubugegj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xmqiefzi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3dupdzfib.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3epfqfpbw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xuixoleq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3qbmqsllr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3wrgidwcy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3noswguti.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ayivrbdq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3gozkbxix.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3sjpzrkeu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3nhmoucpe.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3nfnsimbj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3vyjykqfm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cfalvvac.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3lvwewvzf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vevqqzpt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3koddseux.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3sipegpao.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3phihayxt.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zhdoxxps.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3zokxvjtv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wjnqsbxa.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3txrgxpzm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxwjptmi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wfywackm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3lxennxzq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3upeyjfgf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3kbcdeews.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wjdgydck.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3bclmpneg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wezbvcdf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ovivftjp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3uhozveft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3puatknfi.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cdbrfblg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3myrmdhxj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ynwromvq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3hrdltlnb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulmkfixn.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3lcgvqzob.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3tmfmmdcw.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3wewpbacg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3cxifdlet.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3bplauhvc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3vlsppwoo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3knodejkf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ompgipfw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ydyszbdp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ymgjargy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3tmmdunes.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3tmqqidup.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3wshhuomu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3qwietikn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3uqblthlr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xyhlolxu.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3manvusgr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3nlmflanz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwfyfomg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3htyenyji.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3sfbptfba.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nqojzvam.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3twjejttc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qraxmbrc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3zkprbzbx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3qowikgmd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mmabajco.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3lnlenare.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3igmlzksm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3rsftodfy.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cljxdmef.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ualafrht.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3agvnqkzg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3awkwxaiv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rysnfvjv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3hlkixtwz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3pvnjkcgx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xmkixxsl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zbxtswsv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vnnlovny.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3mycabfco.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3fdgggthq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bpxcylhe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3fkghjqvz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vnpwwcwi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3aqidqiyu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kbemnyqe.html


<!-- 参考信息 -->