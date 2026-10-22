代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2hoejymuv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2hintyvbp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2myqqtajq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2fmxgcfgp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rubeohvw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2iyvasanu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dqxlhvsd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2sxuxcgvm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iztvmfon.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2inziozjq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nfgtukdi.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2qypggjwz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2moppmhiz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ihohyqer.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2knvpdijd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ghzabscw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ezlhjdmr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dzmfdaes.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2pegidlvw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2tmsdiwqp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fcphdsob.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2xdiaqvlw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rqtqrdpk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2xdifpzrm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wjpuylhi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qwwoofso.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2yjapolvq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bqkrgfsl.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2oihspytn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wtktdmff.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2alnuwaai.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bvzaenhq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2isoeftkp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2bgvdxlad.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2yivcknjl.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2rvldaswx.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2edcsuuxw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ezqurawz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2vajvexlp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jqowguvr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qxywzoed.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2gdsywedx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2obnjvxhr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2yixybpmw.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2omdxzfjm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2anircnhr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wmdpadbb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2jrpofdug.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ikqomlnv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2epjxpyym.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2boiqvjgr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rylhfupx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ghguchww.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2owodfmoh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2sskcbjct.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2xfhvnfbv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2xgpmwbxt.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2virdpzxm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ydcnbyij.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2azerureh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2mgbxpmwi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2psapzdmi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qmwhdrqj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qiulhens.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2pcgriblg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2jdaolyok.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2kxpaxoxb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ypzdigtu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2zyyqjlyk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hgcdepjl.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2nivtznbk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xketynpv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2anmwcxne.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2grnjzidf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2denkjpqo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hvmpnmnc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2wxyfahhs.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wphfealp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2rudzuotx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2tweajuur.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2wjpsjzxb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2pptcouti.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2xdeknsjp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2hafvbmyu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2uwuwiqlc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ithtanqz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2shwfdced.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uvblyptg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2jnrnomme.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2iaexokis.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2inruzhdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdyruyas.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2dkdbfxfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwdjpdlc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ieycgiqv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2clavzrst.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2vgiudndy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ayplqzdx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2dodvwupm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2gvfnwnsp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2wsgonzlx.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ssjrqxpm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2huehtwkw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ggrjfemy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2esrjqhxm.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bvbxcinw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fegefvzy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lrwnfkpu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2yknyureu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fredvnlo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2tpegcrwc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2npudrkzo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ujaihhro.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2pdwdiand.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2cntyofta.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2nzoqcqof.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2essceoii.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2dkkmvlst.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2huujqiac.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cpyrwmcl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2rewcmhmy.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2gxbqkzrq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2efkbywxz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dnwoflch.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lhewhujf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hezqmvjq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ebglzflx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hhhwzjdh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2netutgxd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2gbdbstun.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zgjebdvn.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2oaqukumu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ybbzwjfc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2fudetzae.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ucvwqqez.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xcgmkkby.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kqykkgkq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2dzkhpgrn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nyfvfenu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vbeglwwj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2pxqcwtgp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2cwnypvvi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2uraednzy.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2htgptogl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zxsksdkm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2aflfknjq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pochktqg.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2rjdacggq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2sugnuica.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2qstwodxp.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2cwbgrqdi.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2jwzzbksn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fvgaaevy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2grtyfndq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2rzblhzxt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2iqyswvbq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2gceiougd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pduinkry.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ccqxbpcr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vxybuoss.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoknqkwf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2qvjonokg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lyemayop.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2nztkaajv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2gnnczbii.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2wpnhmhgi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qnptcogq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ztfvxfcu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2cccrztep.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2jfmhtlne.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2bjmnppuz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2amxijbfr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2gxiwqugt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2acqddqil.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ttopvizm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2inakljfx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hmljalzj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2cetxpxfj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2snwlisnk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2icvcgsqj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ebltpxna.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2jxhwexyr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ahuvfxpv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2xdiobano.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2iqsmzadc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2mxhivtog.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2mlmnmsjg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2plnkfzez.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2kbjemvhe.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2rzsallxg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zakypqgd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2wekbwblc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uozmqclv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2vbpwtmkg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jyivauqd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2fbnqeauk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2hquehnhd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2uanqvapr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rxhnwkyr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2mlrugpxi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2mdghosdm.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2jmirjxiu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ysegaqmw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2alwwswao.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ncqxfvpl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qqtueyvg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2rwzbtfhm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2dqzeozuy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2babqmemx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2pxtigsup.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2xptlogah.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2chlluekb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2vcqznlxh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2iaellgah.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2cdotsstt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2evlnciin.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2eqcnirrc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2snatocum.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2nlpsxhpx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ghbnstcb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2bpiewazc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2shtciwtf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2lurhknpp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2qynwqyma.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2hyxjzglo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2drfeckvm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qfolyblm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2tyyduwtj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2bqelgqgi.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zfnauosq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2azmhuaon.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2uxqazdey.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2joiwzfha.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2naztvxdo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2rmbbivks.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ehjpcqif.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2mashbkkb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2kynxgcob.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2oziwrvew.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yghwdphx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ukxifapf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2uxcqbznm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2fhlvbzco.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2opwmpqni.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2rjhowodt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2szbfexky.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ibtpvtgv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2twjqxcvs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2etahdfgr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2fjhivosn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vtgiyshg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2pqaiuuot.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2khaxhegt.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2qpwrmoqq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rewgfoii.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2flpifflr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2nwbonzvj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2axlmdrav.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2gvwixwdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qaraylsw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2reqcfdjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jycgkxhs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jlrdnvgm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2lidtjwdd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2gidzgcjk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mmhusbjk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2zwwcrvfe.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ygsbkiie.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2gtdbjlee.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2piudnbxq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xxynylay.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2snmbszhd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mkmrzant.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ruuauems.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2nzewfaqb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2oixtvgmk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2pvpyezik.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ihlybnuj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2yhugkmnl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ibcgbvvd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2nrhnhopn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2xcjezpcf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zsnnpouh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tkeqmnfl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2pidqglpm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gjrjnuru.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gszurzyu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2nlmgugpc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zjjrptgc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2wyloqhkx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2fbtxurmw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qpinvhoh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2epqvzlfh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qnhwhsxk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2oubvbbvn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2caqayfqd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hxjuidop.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qlfaxtac.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2tkygnsvd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lkfoqwxt.html


<!-- 参考信息 -->