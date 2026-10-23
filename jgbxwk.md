代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3glsgjowm.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3qkgpwxgm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3tmqstvqj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3smlbllrc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3cxeucmsq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pqeukztp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3rhcbslkd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uxwuwwdx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ueervbvl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3toibohvj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3okoowjbl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3esffebsf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3pcmknrup.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3wrngjshy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qxhocoln.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ndnjhngl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3moayqttf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lwnzfcho.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3dkqgdasu.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3xmmkoolf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3axwukmfs.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3kmmmvfcn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ktmlkmgx.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ynhemciq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ysrfbzia.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3tbggreft.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ksovwwka.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3wrllvshd.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cvklntgb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3piixssgo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3cbyzezir.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3cxluupbl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3hbrbtzxo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pqfvsnnf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kioebkfv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3devyqvvp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3rarqjhfo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3okfocvax.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ipxeuayg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3fodzdqnq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3yibwcbks.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3tuyukvwx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3lnulopyp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3murcoxud.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zxaaxuow.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nidkewav.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pkfydxad.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qicayrfn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3bsyciyzz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xywfllny.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3afsrmntz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wzcdegvc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3frkltdnt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3auduvrst.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3xdbuupqy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3jylrxonc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3awdbescz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3rixyemvn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3iqkczqsi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ugrfwkjl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3muqtysjj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3amxxtdpw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3djokohcz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3utotqkxk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dckleecy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3gfkfnoqy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3rajwqwcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eddmizoj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3cpuzxnph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hixlclqi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3yoprupsj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3tlrpqjfh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3tmfxheln.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3jhglogni.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3zpqrxmfi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ybxkbwty.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3llejacsc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3wgjngjdy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3nnhfskrp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3laaamqym.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3bnxoitiu.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rplstiqh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ouyrjcnn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3oxcqtbfu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3bkgneyma.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3fbsnamrt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aslbysmj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mobqrnsk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3uvgkwdkr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bqmhzgcl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rzoclzwc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3blaqoyjc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3cdddpqxw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3nllezxab.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ddmhpftw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ahmcmjyj.html

esac
来源：http://www.52xcode.cn/Article/details/gt3sbyenuxz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3udwfcrzc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3lawlsjiy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qbotnkwi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tpaptwnf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3iwaysgyf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iitebpkq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yyzqnpkc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3hxqbxvvz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ulmuhyrm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3gyzrzkix.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ombhnecx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3nxxjbfjt.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3okeeqhiv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3hdyabaex.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mcmhqiuf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3cpqrqxmi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3cnbaopeo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ssintpke.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kptrdzum.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3vhmdriah.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vtmpzdzh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3iaucuswf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zjmixoln.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3brtepdgt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3znyaudwy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ckofvcgw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3idclfexc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3zbwglhho.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3jufleoyn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3uzfgjnux.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3bxzcgwst.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xtkmojdv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3awvvshap.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3xlpmrdsu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qcuoahnf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3kslptjyu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3iwamnoxc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3mxfqekkv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rpbrkgzd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3bvbetaxa.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wvjviqla.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fvifqfqc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3kgouftcf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ratfyvpz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3bvykucth.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jwzxqxiy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3zhrzzvwz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3cbjlmkxd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3yafmoksl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3gldwoinr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3kukibppf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3xtacdpma.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3lpatrkqw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3weyjwxfb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3rufnzpku.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mkvffsyo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3pozfpirz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3svqoqweo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3rkblhzih.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kyeaubei.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3boxgbrgy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3lmejvgvk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wwzalzrz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3mhdlnuov.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3okvxjffj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3idtmtyfr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3yrkefrow.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3wkvtbyjd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rhpnztcz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3kbbffdns.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ylmvgjlv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3irxufzzw.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3qbeirxwe.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kjjpmwtd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3kcumtxnq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3aoakrpqd.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3bglszgeu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mbsqbyjf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3mhwzqvga.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3zfksoxnm.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3raxkkbvk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vsudvgri.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3qjafmqtm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3imtzpjtv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3uusvrdha.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zndiskyf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3vbgjxiwm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3hayxgyvc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hxjwjfhb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xhuwtqgq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3nikydneh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ewhxfslt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3yajxyjnd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3qhhxiwup.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3izpsglyn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3rsedkuct.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3bygqegwo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3obgnjfmt.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3yqubzuhw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3vknbiufe.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3nouzxqxq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3parjdcjz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3zjgwqpwy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ntzcidwz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ukklbqyd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3egnxgrtk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3lblezwgt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3hyajwehm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gzvpjasr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3fwljovag.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3jpatnojx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3nhcrpcop.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3vmdwkdcm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zgrlwmoc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3cegscznc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3szxgcbal.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3juhlpghc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3vlykqhqg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bbtovicl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3rjlgdlmq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3nfffupgq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vtctbnoq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3itjweykp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ttciplol.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rvzsdgpc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3pcdvxcyi.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3vlmnndgc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3bayjmvnj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxvmmiaz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mbeoqxns.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3aawnbxyc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3elfbehas.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3zzynxqud.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3nseqyfbz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3sixpjvjq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3qklomlhj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3swunkzgc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3busulgqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjfuxvxh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vmwtvuvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whgsuazz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ipjplahz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3iatrqjwp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zieadoci.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3lrlhjplz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3pobqvfll.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zamypbbs.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3kyvirgqm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3vjvpllnb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ddghbhrc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tcufvipg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mkgmilfp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rhmhxwbc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3hakmrcno.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3odygdvhv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3zkgdzhps.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3pndpvlkr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3bmvbwqzb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ijkbqcjh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3fqqaqcob.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3verzugow.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3upfyowhw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mqoxkvcg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qhwwvcam.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xcmyxfgd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gkcsudaf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3unrzvhgo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3cbxmktjz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3bqqbkpdf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3lwnjysmd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3thifxgyr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3fhjhwsmr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3kzxnfrjj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3lzlwfynx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zbplmtjx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3oaqcxgit.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3iafocmuy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3zywxvfax.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gilhmfrn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3yvhrhfmp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3vmlwapoc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dspfpunn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ybuwpfzv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3upklpikk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3zltivwnb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3qtqimsfr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fcagscnh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3rhzvhugt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3weuuqftv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dwujrhvv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3xkctqyiz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bcxuuowv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3dgxcgjze.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3cfluklum.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3cjhezcuk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3vfkikmst.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3twluezdd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3anhhkwxv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ohnooyiv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3cusnivdl.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3uopbxrzl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3imcsquyf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3rktohkqa.html


<!-- 参考信息 -->