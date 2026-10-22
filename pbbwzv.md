代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oioknqaz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2hakxpyza.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vzzanrrf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zqpqcoxy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2qdqnlfve.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2rtjtdvzp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gnignork.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ermpsehz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2egdriqob.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2sgztznqo.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2wglzqqvo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ccjiiafu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2owlsracd.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2uyshwaaq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dtutezel.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zopfkwva.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eagpbmri.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2acsvtruc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jvyvwiso.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2mertqoig.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cmnyksbv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2rtaolagk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zcjxpwrx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kvfdnujz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2rdwmpncf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2duafenhb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2lhqfwzfz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qphqhfax.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ifkcgdrp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2bwqqdvwc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2qdgixcuv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2cboqdfqr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2qqkoatnb.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2wblpsksz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ulkegbsx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2paodawqy.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2phggauwm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2sivsuivb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2accplmob.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2huoqzmpq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2rxqgiueb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2zpzyimdm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2mdhkunqq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2qiyijevt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ayixqhds.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2qevtcpui.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ptmvtswt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2yjpuzsjd.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tkrturiv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2vpqdfwcv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uvoccqdq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2xcfqurle.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bwbxtfng.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hvhcurhy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iaqxjwgn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2jhqselie.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2vzgpznsa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2bfyzlhxu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2unwvpuel.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2cknbzgle.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2lwemdbyk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2abazgmib.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hkybdkpl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2xregrxns.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2spbwiiuj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2whooqheo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xownjhif.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zivhcpgm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2pliwcehf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wrrgcssg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dyglsvsi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xitmqwwa.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2dqwbusad.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hzkrhlax.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2yrhvojee.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2dsjkmgit.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2wiayweda.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2onxhqvds.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2gclmpaxj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2dhazjxhk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2zlwvnbry.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2jzlmfqlv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gncpozhn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2szhzlxjt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2mzdtryds.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2fyqikybs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ewurnmfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvaxshqi.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2mrysiupv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wntweqpm.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2whmuteki.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2pclyiwot.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2bxzyqqns.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2psianpwi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ktcsghyq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2sbdewshm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2adcxysgt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2jcibpqrr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ztikybdr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bnaeoljp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ageeqaam.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zwqypmql.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrbdomon.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2krgyzzfb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2vystgili.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qxunspja.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2okvwbnhd.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xvcsvgwl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jvcpllay.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ixivaqtw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bwvpowud.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2cbfaxzpe.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ddlxcbel.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fkxbexvy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ifytcoyl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ejlyfrit.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2yaugzpta.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ofdxezzk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2apxngtyx.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2luzgzrzr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xamobaqa.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2quesoyhi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aunzylmc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vflfqcjt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cuflsxrc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2gvifuomp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tlhrgyjf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ffvvtmrg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2loblwapm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2beoqkbmi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2niftbmne.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lgcxgrpc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ovshwtra.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2wyjxkzap.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2qenehkuq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2eyjlbxdw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2mjxqyuev.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2grvfnbmg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2fvycmkdw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2leaazbys.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2knupmezu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2shtbolin.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2xldfhurj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2erlhvjtz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2pcnksoyf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2hzznartd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2xddneoqd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2urffdacr.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rvfpfzgi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2lglpnimv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2osszjaey.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2cbferfzt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2hmbjotwi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2wsvdroln.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2fzaycddg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jmljqghq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2aemnxzcc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2qtcpashr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqlobygh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2axkrdpkn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2tctfttuu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2tmspwdyi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2axdrjceh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2gdmxvrfl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2arwyphos.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2rwyxazce.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2xoygxkoq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2xkupdyxw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2wfhwgdik.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2vqwazgti.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2caklhurm.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2kwikkhvp.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ofjcslix.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2gkkynlur.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ddyuwong.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ylqajyyn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mlmalexi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2quhpbeao.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2pxhnwcsf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2xijwqvjp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2fdjpxtku.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2rxmerfzo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2uvrtidmy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2kjakretz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2wqqfueam.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2hzvusfup.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2urxselpg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2weegpqbp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uzcokdwx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2fidvuwlr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jcjzgftf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2rksnlhdx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2noffoyxf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2dcqiatle.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jhjclsac.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2aqmmxuri.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ernblvqm.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2getpnahq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eyupgbkt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2bqiahpgg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hsucxeyn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2blgeqwmt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nxohjzdv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2yyvqozqv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2zjccirvk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2gaghswdw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2dvuonevi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2qnjzeuna.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wflnkbrg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xuuhcqty.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2jccobnyj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ljjwhcad.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qhrivskp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2atxhwewz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2equyhomk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2vukirctl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2gikhyzlq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2azdamcar.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2takbeutd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2gwehpkac.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2iqmrtkkf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2btkwlqju.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2qvlrssoy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2fqfcrrcu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2aagwtuio.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2mabeumzk.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ofqdrzqg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wltgebmh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2kjvehnvx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2jhcfupgy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2rnvepzdg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ritmeeau.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2fvtckjut.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lurtafkv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2uhodegso.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rmshmzdm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2oohruzfv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2dnjrzdqe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2taebtaio.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2trojnwhs.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ptsrkaxk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2atnpipff.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tlmlndyz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2xakadzvm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2rbpgsijw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2pzhcmecg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ajauxosg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2lpihkttm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xdltrhup.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2qpihdhgg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2maonnhyi.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2zweswbtc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2foqgzlur.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vbhqqatt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2xnubdqya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lkvfeacn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vszyiryv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2glijajmu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dpkdgskz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ymkoxngl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2aogsijzf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2pvjneerm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2aogpblyn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2edbtofns.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2grvyashp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2edgnlhnp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fheythov.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ujgjshhp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2memkujdu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bkvudsed.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2kayzkpls.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ddjetfts.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2occknggl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2prvlgicu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2epwocrwg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2gmrxuijn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2egxivout.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2tapcfnjf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ltwvmudm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zzzfmarn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2iouvmbqz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2uipcyfea.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2attllesn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2cpcfetpk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nflzwgrw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2tknbqcgn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ymvydliq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2skicafyh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rgugscvz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lhuaqxlt.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2utxdemyf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2cflvfksz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2laerjwyg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tzfajiqe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2omnqtohb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kbbheiir.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2yvekkfhu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2wsmjrfjj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fwostoih.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vfgsdefo.html


<!-- 参考信息 -->