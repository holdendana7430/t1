代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2rilwvcas.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2gibtwucn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2yrdkobjx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2nsnjpaxy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2cyntxkew.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2xskeuipq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vwweexkp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zucveorx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mzntbwwh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2lctwcvkz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2redydagj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uobrhvqn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2tlvpdvna.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2kfvsrxbn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2tdgafhkg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2fsejzhmo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2cdjyoeut.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2hlyrmpnc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gmsfqdag.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2loxequkr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wgejurmn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ordjmatj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rsvfxqql.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2hyswsczh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2xhhivvst.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2rijwftvy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kvdyqlfp.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ryteodbb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2loqvvoyg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ktzesvms.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2feqvfjds.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2qcfxifcn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kyleguzg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2nmchjcro.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kyaquwlq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2bqhvsrfz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ylvmdnvr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ldcdmbrx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sjdxmsjy.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2qcppftfn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2glalkoem.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2fuyhibhj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2jcrzuvtf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pohjgmez.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2cogsphqj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wdnuabth.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2pcjkafeg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kqvwimsj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ghuwbzls.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2dilefkod.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2rnxyucya.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ilmbxzxf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2vxtyjcil.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2xxfxkfjw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2yirtpuij.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2hdozfbqm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2wdfkvfjj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2pbootxrp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2bkokevqw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fszybcwq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jdpoujoc.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2rnyumedc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2eexzwbkw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2eoiilvte.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2efxzbqkp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2htitskfw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vixkkaez.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2gsbzpchp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hlzsrgqc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2dnufqdxc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bncehltq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2mwjoyaae.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2hljvjzhp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kcrbtvam.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pceadtfu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2pltjecap.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2aqjpsvuo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2rggqapwb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2vmckaysn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zbpwksgx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2nmkxdbsf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2qzxmhpml.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fuqxcdag.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2znsgsrkx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2whddhopg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gzlmpaxt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ndlmjoeq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yptruvuf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2umfczahk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lwdvmgto.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tbomrvqi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gcatllbv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2zlvsvrgw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2upbsirxu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2igckldaf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jhiduglo.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ltckueqz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2zarppxuc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fboqskkf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2dupujctd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ohzshoso.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2qrmnchna.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rxmlsfmk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2baitgowy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2jrgzespg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2eharetqf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2wqoicxax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ksypzrrw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2aqsdjbxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inkgmhfo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2unzxdvpb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2fwtpkwrb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2qhtkxqbf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xjbedbxm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2rebswrbg.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2wnwhrwnr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ebqgcgbr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2iscqnqck.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ndhuorgo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2bnxhovdv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2kuroxecn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2netuxyzk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmagvcgx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ugozyvuf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yedgnten.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jfydiovh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2npnlynmy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gjdronzr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ihbvduae.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2nqyhartd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2effalwvw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2gvvcjdgp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jgnwdicd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qwgyzoac.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2mnxoqbbz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fiirgulw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2lbnikbgs.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2dpobbmft.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2akznfjuv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zpjctqwa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2sqrqvhyg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2oulbpyqx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lcrlrjmh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2syptszfa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ziqvemmu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vgvbtzif.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zopvfgii.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2mzwqldpy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2tqdwjtgu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2srmqhiva.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uekyxtkh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2suwjmlxl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2krzuggkt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2aploikwd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2smdnytzp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ykvtzusq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2rqjiivlc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ofsykrmg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2mhhkypba.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rhcsiwts.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2juscpluj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2yupvsiyp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2tmwbmmao.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2awavhgbu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2escghyda.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2luoqltwv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2vvxwidkh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2hhyokxfs.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2dvrpagtu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2qwypiwrs.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2zavxmywm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nmrflwps.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2pqdfurlr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ocqarwpi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ejvldosn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2teodqjqa.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2utpnkozu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2wpaaltdw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezegnclp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jrwsntlx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2wrokdlzy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2otygwbvp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2sccatdxl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2cvmauspc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2oljfjoan.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2flrbvbli.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2pmldmeen.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2nduyerlq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2nvagiqfm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ietadyyy.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2xoexkpcu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2nznhfwbn.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wfzhyxlq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2bmtiiqea.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2dqtbcuuk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2cdzmtglx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kftvatih.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ihbbwjuw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2tmzxaehw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2svotlpdn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vpawfkyx.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2euaxalag.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2kxishjye.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2byhsmjln.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2hkkqwwkp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2prxwslsa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2lbatrbkb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2cjruhkfu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ksnosmlm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ubisyipm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mgbeomgp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2wtouwjcf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2vofjecgl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ybyhfyqt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ckkaahiq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2jyqqyhnh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2bsmqbzhd.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jkqwxamb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sdnqovgs.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2mcrzdnfu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ebfpqifo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yyyirzaz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pmjkscci.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2fvgelssx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2edvkppzt.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mlwrfsbk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2igbprgpg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2izsbzjtk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2vkkgypeb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ngctgalf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2yduvwagz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2macetscg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2lnrzqqcd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2endrhmmd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ruvbcdoy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2srfwlmsb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2hfvztdro.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xxzlcqeb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ctmhtwtv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pmprlkol.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2vcnvaube.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2uksmmvpw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2oqloiiwu.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2xlqminfp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2kjkbyrtt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2mgzhclhw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2cezkfwom.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ddgkarku.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2sjgvbift.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2buvzrwyu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fgcumdgd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ruxcbajq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2oyfylmue.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2mfflisii.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ghzatrqe.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lxicoxpr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2posysotj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2tolvcsxd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2fajtgwnx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2decsmzfq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2wcqctdar.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2qadhcxre.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xuvjdulw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kfdeoghs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2zmlydhfz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2dienaotd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lnjfjyqk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ivtbbnif.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2agakdoqc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2awurocjy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2lrmamfsr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2idowzjhk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2kdyqpprx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2tzmmxsxa.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ykdqhgod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqmnyogv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vxtaqkaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmyuojln.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hmpwmrpz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2isacrrxf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybgapwvu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gfnxrhva.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2pzrwghzw.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2nrqxmkxj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ghokivfh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2upajwmqy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ewoygtyj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xhjyxlmz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjsyfnrl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lmqoooag.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2afyvmnkd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2surhrduz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ufwprhmf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2zlahhtpp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2egdmvxjj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2osywdgqz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2hwmcvbsw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2abugnpbi.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2pceyomof.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2smwdetfe.html


<!-- 参考信息 -->