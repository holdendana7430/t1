代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2kxleabrx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2nzyjznhj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jucgkpjq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2jytkffcv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yrqllnyg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2daoaxmfu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qqacywsp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2lynskwpi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2yqcbizdq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2muktlysm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ozwnqwua.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2zwrnzgjf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bxwiwbvf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2nmfxdxye.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ndgehmqa.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2yewydshx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fwfqjzrk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hkxixano.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qpztnbmf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wzhutrse.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2efkxvkjj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qhxebzja.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2azmpqymq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2kzmybxbx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ykpfxady.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2vhqwqctq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2sthbxads.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xizskdsj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2kynuwzms.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gvrrnswp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2yyclrshs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ikqhwuos.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2rtfjxrqm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2cmdkckhc.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2fgirstyu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2biykmhbr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ewdnfedi.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2izjovnng.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2peazimzl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2xrdrvusz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2nkzuetak.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2evosznxt.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2uadkwlmh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2lkxfwsfa.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2mjhdryys.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xkocfxvq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2vnnhrqjp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2qhdcmvrr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jpviqalz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2yhptiicn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2seeybygq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2yjxgoxjm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rnomxdgv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2arfzalaz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nzdqapgd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2mzkordpc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2adzhbkpi.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jttjmery.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2haluipna.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2mkbzbpqq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2chlyvetd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2rdsdskqo.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2dibkuvqa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2rcxlqmwh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jzwaahxv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2abvoafgs.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cyouzhxq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gatoyuuu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2vnocdymm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vfrtbtbt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2uoibvezv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xamxhads.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ewcvoabq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jwxpkjgm.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rrmtgawr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2titjtnnz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2yssdtnkv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vbcxecvz.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2jvurhlsg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2wreearlv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2bihkmyby.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jzabarjx.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2nhomelno.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2wvnjtjlv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jxmpmgmq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2xratpvkh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yntkntag.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oipwsgqd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2dnsclbhm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2dufadcea.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2cjijxxpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihslehfv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yohpwvme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ssosdpkf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2koruoloh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2eegjcomb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2gysqnnvk.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2lcofhblz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2xtfchsbj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2hgaselyt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2mdjfvxdt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2efryiqjr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2kmieblcb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2txrlmimu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2delquebg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qcclkhhg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsuaubeu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2kuwntidw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2usukwbde.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2smddpvaw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fvycnrca.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jsmcsasw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ypasolnb.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zkpqswls.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2hrkfpcxn.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2hezknama.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2miuigagm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2iujmknsf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2djfuvely.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2eecllvcf.html

esac
来源：http://www.52xcode.cn/Article/details/gt2krqhxigq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdxclwxv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2nlyumlkq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hdiehzmh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2swmxxzkv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2bpscxpph.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mjphnrvj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kexvpatg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gjyorhud.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2cmkmiskb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hfwjphaz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2qidddisc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2qobqwgtn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2jnjhldkr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jjykbymd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ivqnnxip.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xckxcwzk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qqwetvxa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2gdytucdo.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wkkpnrgw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2tjtfeorr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kyhmqtcb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2dttockbj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2bwmfzwoz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ptzhwpnl.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zvvfrvwr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pbyuuztu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2fbtvypai.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2peahaqzw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rgdulurv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2sjlgubti.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2zrcgkusp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2dpmezovd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2fooalonf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2rxuwwheo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2oekspvyv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2skxrmfmo.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bglmycds.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2bythlbvu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ukarixwj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2yhivkmkc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2hnzpvtwq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rczyktgj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2thfbroyl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2rrjpxcna.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2qjeredgh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fybmfbjj.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2eitppyoe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2xwlywvey.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2qmncumxc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2lzhyljcp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2vcsceinx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmbplmae.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2uxojenlk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2gdqdhmpw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2dxaqlqxw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nvgogvbm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qzhaynkz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2eqwetois.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2octvonam.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kwaocsfe.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2mqcgscjy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2effdlymd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqgnwlkv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2peiafoak.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2pfmdnntb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2rmpbawmg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2mtyeptso.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2lcaxdgzv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2pqyswgwa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2mxpgdffh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2szlzewkk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tgbqtwvl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2oaqigmvr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hcvplqxy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2nigcfber.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2cndkbhvz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2bamoryvl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zszpmgop.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2kaexcfca.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2mxpefclx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2yybdqhvv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yqcdniqu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2afjmbosr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2kwafqabz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2youmxfpa.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ktfxtuxm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2oalroclu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2jvkdmmjq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2madqmxhf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2botzbetv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2qinybfjc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2wyzinyih.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2trqygiyc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ddpaoafq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2flgohhvf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2gxteowcw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lniaxshg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ppkhufln.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2chvetiwo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2bnrbblhf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ajyyyezf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2cenhvktw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2htvekibc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2galfaypb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2gdfcbzfs.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2caugexib.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2voqgosgw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2tkdfgfzh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cxkykgvy.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2tcsroeuq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2jvhfjmja.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mxigzfmk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gpfwyecu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2zwxeofqw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2qqajgwhh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2pqrbahnc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2wmouowyl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2sxoujhqn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2aqpfihvp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2qpysbcup.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2dmchhjvl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xsdrafmi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ylgnnzbe.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ncgmtutm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2wbtgifrg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mouruwge.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2tdpnzprz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2rujinicb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ecmwbngc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qffkexnl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qxmafoyb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2etrjfjda.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2cftvqmms.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2jpkwpzdg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2hlovfdxy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2zexrgjol.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2sddpckdm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2azrwywgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vsokggrx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ddsfsrnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nazstrzx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2retdgdqc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2mtcdetdf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2vwqvpzjw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ycsygsfu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ofesvrho.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rigmucgy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2mcxlhgup.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2vxlznhza.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2oqqrtmnr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ziygfqto.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2beajqeol.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bpbtdrdp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2vyzrxhmi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ehlczavw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2gfxrpahq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2niwiorml.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2bvbcqlxi.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2kkogkzdm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2gtuloawl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2gfgixyet.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rykclvhg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vctmioua.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qrynqjxo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gejjfvwr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vuzzewzo.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2kranukxf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mctzelbb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2tcvpidkh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2qeasbfxn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2btdbirro.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bwwmegba.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ypcsmasr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2vwtiifjc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2gyxowfpd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ngfisebn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2shlawqip.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2fzarxpwq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xbswanle.html


<!-- 参考信息 -->