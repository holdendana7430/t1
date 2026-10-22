代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2yzfipvrk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2oshrurik.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2gdruexlg.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2uhtbvfsl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2udsxcjgo.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2hmopaqvq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2hsroeksl.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2evtuokck.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2luntebrh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2nzjismrn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mlyrfope.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2lpnuzjcn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zgoyudbu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2rtbpavmg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2luoshcnf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ddslgsww.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2jpgwvdxt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rfzvgyub.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qpzagmhs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2tefeppja.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bfjxsutv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2nxyhuvip.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2pthkjmjs.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2dxcdjblk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xgjhwbdk.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2adeewcaz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2drecrkrn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2vmxszast.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2lstcdzxe.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ysolzuca.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cuxhuzlz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2xuvvdpvw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fjetehcd.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2tcjnvdhs.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2sypajmmr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2pfymolxb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kvpjyzhy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2fneubkyh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2trjoxehy.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2aqzcbrxm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ahqetacq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2fknjcnhr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ltstujjf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2corloztq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2anetkryp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2gjhpqzom.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2hohemfgc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tjizjcga.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2zcxubagu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2spglecwy.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2uostvmkb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qphabfra.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bbcanmjn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2fdegykji.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2cpgusiyx.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2wyomtjej.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2irtvxeht.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2jxcnfxet.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2sudipuof.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2gasifyvl.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2dhsqakmc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2wfcpkhym.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2rrsqyrjb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2hmmidysj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ftgcjnew.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ulzufqkg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2fwonxotd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2mkkksqya.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2qvbopsls.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wjtmhmwy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vsxbinbw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ghbunjpm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oxrlflej.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2qqkxelqk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2alwsnbco.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2csxerstw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2mdqbtctq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ncsmerur.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tpungepd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2shxpcjqj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2tttbsylh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2gasafttc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2axyuumau.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2vvgxcucj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2xbzfvdtp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2sjdqesbq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ashuxnor.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2fwhekwia.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2jwmlvgpk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2foiewnif.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ewsnafbc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ohhfktdq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2xjjjhcdg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ubnzfbgt.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2yjiplqvm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hvuezikj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2dibcdhyl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2atgwxmpw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2kajkmnit.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2gtcnkuot.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2khoeximv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2hvdpwisx.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2lzwtecir.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zdberunb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2pawyiztl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2iufpwqdl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2chudumrq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2mnwcjffe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2woympmol.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2hfmdornl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2gnfjehps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2henkerlb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2hkozpkpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cbbybwgf.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2kuoftzsv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2yttjjqmk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2enzgkgnt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2kmcrzure.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2trovetxq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2dzyryblg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2nuwqmvin.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2nxfxhrzt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2tgitavxq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mofytnbr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2pdsfgudo.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2yyjfaezd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dbkvgoqy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2gwedasje.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ihtlybzt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wybvcpqq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qcwyxlnv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uyhrrpxc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2tpoprbeb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2hcfqwhdf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iioyhehk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2bzvsixfx.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2wktjaida.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2qdqpzmeh.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ycajneyz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zgitdpyc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2quaaqmje.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ppthkbdv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ewbasyrk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2oithcwjk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ikrdsqaq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ohjeyftb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rvugqkcb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fhqsxbvl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qgvoujvd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2mwssrvry.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2trrcatwb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2nambyqhp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vcjdjkci.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2jouieogw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fcdzzoea.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xxxhhugn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hwzqmpai.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2glmveuoi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2vxzbtgco.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qjidgmei.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ekvkttqx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jveumpjk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ouwvrcuj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2bjuurvxv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ynpsrpkx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nmqhnyoi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dnjncbwb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2eyhymvit.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2armciuji.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2fpoojycs.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2dgkrjpes.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2lvazuyjm.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2gtdnxhkm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2dfeandee.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2akozxoit.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ulneflwo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ijqcfqwe.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ufwpuoom.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2lshpbixp.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ngcuupzk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2edscbjkn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2phgweomt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxthrblx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2vvdmcqeu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ifegfjqz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2aklpnxpq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vobkwlyd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2smjzxszc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dvgmnvbm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2thlpcaeh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2gvdrurjl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2urtbzcdt.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dunmxdsj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ppobxwmp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2qyqebhzb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2fmtyerlb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zgqxlnfk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2hhmvetqz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2kkwhgarr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2jzttzyqm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wubvjzam.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xeolzkiw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bqaynjhp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2dhpyxujv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2rwxazkln.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qlzmllvg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ptwdguti.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2qiiwdcub.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zrdnrkav.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2plsqsvfu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2egknuunf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ddsfnkxn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2raeoygld.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2vadmzctr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2owqeqzie.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2wqwniekv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ucxiuknc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2yftraxyi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zecevohi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2xcsjpnzm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2lhyeqkqb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2wnvxpxac.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2daraloig.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2aupmorxp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2vwpkzxzx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kwgctpeb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mhfngaco.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ztmwyeiv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2zmpdqiud.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2bywirjzc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2erhousyl.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2alpukvek.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2pzhygytn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2atvykhrb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2wusrhyqu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tuhidokw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zztimwaf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lhpgpvdd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2owhisdpj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2abwlvnou.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2vzvfcumo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xklkgfzj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2tjewauhe.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2odaghtbo.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2oququobq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2nuqbtbcf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2dkcslqnb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2jnuafdfj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2jkmplqer.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2mvqoaoof.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2idqkatlt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2pxbwvmxw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ectcfwrw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jokgfrkn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oaoglufw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2cxogujwa.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ntpzxzgt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2afpxlxfe.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2weitfvky.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qmdizspl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2gdjsgpmj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xdvttrpp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dtkcsdpl.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2wyjkyejn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ncqlstcl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2izsjvdhf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2uhnglozk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2zetagkbg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2nzrsesqj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ghbbgsvk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rmuopvro.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2etgfmncu.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2cgecjymm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2euzzoqjr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2tapcyeju.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ssfrpbrh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2rnioifsl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ixnjpqxh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gsskfeks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxdpoyjy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2pznvaiog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dpuqbovh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mzegzrpz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dueeymfy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2veichtkf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2dtvsqeqp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2cuqppxwa.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2alntrfdc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2nptyajji.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qahiiawq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ayropyof.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2djatifii.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2yxlbjukd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kkfuxsnl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2fyfsduob.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2uccvycfq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2qopvdxgg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2cnosglbz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vcygsjyl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2vlttwpac.html


<!-- 参考信息 -->