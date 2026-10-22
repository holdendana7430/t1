代发 wailian999

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2nltmknsb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gnljvpvb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2fpbhimtk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nviglpuu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2xftbjieb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2rxmuiwos.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2vkpilyey.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2glqduash.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ewaewoav.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2tgqpxzcw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2brinnxit.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2khsbkzix.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ycfeergb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2vosynxgo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2jhbktfrp.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2dbdkjfkz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qfvaaxcr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2cujzcniz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2aaiapwwo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2btezgmje.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jtgtqkso.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2tznppqfj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2gqukpwxy.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2pqvwkvay.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2koaxnokb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2cvlctxee.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hmaoelhf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2gqyuvyjq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2hkfmzmdp.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ouruhcne.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pcipommz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rcfkrbzh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2vbpbvymq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ssddgmmm.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2dnfmmatn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2jzkxpgfr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ckclsnwh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2zutxuqtx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2aryofkli.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2iiexiqwk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ksauuygy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mdnavwgp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rukfupta.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zuzeawza.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ipucdagb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ompllpti.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bvjlubvn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pogiwkkz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2albvkekm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sissfnmk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2idcmlizs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2gmixwkdv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2plxzdvci.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2pxbwllhd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ngacqezn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2yexfwwds.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2fshhbnrg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2hoibismb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kiurbcbv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wgqoreos.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kxmuizhg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ealjwyaa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2suzhptam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnanlymg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wfuryetr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkfleonr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2trypobwc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2vppoixqd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2hjtyxnem.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2eckikjkp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ikqymrmo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2zxjotdzx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2wbqboocr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2cjvnkabp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2bxwyvgmg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2vkayncwd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2aubvfzzu.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gzgrjtbp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2obtmcqnz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2wpmotmif.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2btlvezxj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2uqjfzbii.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2oxfkinlj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gfpanpii.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2zblnqrbw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vffkrxah.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fjxwsquj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2yhnllosq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2vzlbkcea.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2igdywwho.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2aycnxggl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ytalyneh.html

esac
来源：http://www.52xcode.cn/Article/details/gt2paocchod.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2yehugltj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cyatlhgd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rymjxhkt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vmlemmcl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2lczphcar.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lxeqdxmz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xpjgxitm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2urgyghtt.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2txdzmxyy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nebvywjy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2nucxzhem.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nflciyyd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2hesnjpei.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vblzkeah.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bulmwiwc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xfhzcgak.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2uhcrazmp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2zpfdzxnx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fofqfxsj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2pjodvybp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2upwkhlqw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2pspcxreg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dxymljkd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2qkcphifv.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lkqyynao.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2oamiyroi.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2lqwfhxju.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2bikzdpzi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2niuswmjf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2cxclzeqn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bpeuyskz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2nrrbonzp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2aqepwkxd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2qkvktoet.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nzcldxxb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2djumhtaf.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2zaiomyld.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2dwvctmim.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2eskboezb.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2urmnesra.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2elfjahlt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbtmeprl.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2tplpzkhj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2coiqbfyv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2byyhqzgv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jdirjewf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2purovptk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2lefaaaou.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2acbzlrjc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2wixsyxos.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ifisxbfh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2dirnusrh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2vfsihmcj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2sduiwmto.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ftraflad.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sawsxyfi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2tqainnul.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2pkprsdlw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2iqxucndj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tgbaevti.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2hbrabpak.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dmfgqszj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2skesndpi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2njgmhnay.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2itabosbl.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2lpionmis.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2alvewjhg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2bhwgghgq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2trykqdzp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2tnxodqto.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2zpzvpmxd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qtkuumjc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2sojrfkot.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oayutjid.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2kntcuthl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2cuzzgssb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2huffsgaw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tyeihvlt.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2naulsfey.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2swjfexph.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wopqtlps.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2miqburvl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2kikneytg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gheiuljw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qtfcvrqp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vejzysrq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2snvegtux.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2vtxvnpfz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gijypcik.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2dmlptlpz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2mkazibmy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2uiacbvrt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2jbfneqlu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2arvlqyuj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lksvscll.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ekjwtxci.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lqwbpnvl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lrjrcrde.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2rljxcdnl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2jvfiwamy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjgqbhbi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vhavwdjg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2btjfncme.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2kudhwpen.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2oybqmeab.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2jxcqjcrt.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2hjwqvfmd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ydsmzzia.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2mctvakza.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wckvjvqu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2yyilonyj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2quujebxg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ubjzladq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2hawhqtev.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2kffbpupy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2oejfwebf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ukvjohec.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2vnkhsfkc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hksiqreg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2gtwrbtfq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2pyfoiely.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xjsiubra.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2mrtdzrrv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2pglkqpsy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2etfgmzrh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ayftabfp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2wklezogb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2auurnkup.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ersdvwwf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ajeecxoy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2wdokrmxd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ahnshbxp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2abywhyhj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2cghladgz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lmqvxoya.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2gzhdcldx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2lsbkaauj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2rfeglmsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esfbugjy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2dipzuybz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntlvjfoi.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2heabrmfr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2muybukaj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhrdothp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gnsdfgjr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2xmqitvxf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2gwklnfvf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2snrpqlft.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2pjqfobuw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2wiopbtgj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hzamfreo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nosgzvvd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2elrikrfs.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2alyksfyq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2jdbjcyuv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2btbddown.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ggzqhoah.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2grzsnhqp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2exaqckoz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zwmetxic.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2izqkebwo.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pmxnweay.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2scnevzjk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2yumbsbhn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2agyxdfld.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rlkbgsso.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jscpmngm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2amafwdbl.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2foeabawx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2fxghkijc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cudbqmse.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2neozehkc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lhsfdded.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2znequkki.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2etiicdiv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2qxeesqtv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wwidphee.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2aawavigk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mqrnvref.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2hlaquuqg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2fpleenbn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2alhiesis.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2igvtylon.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2scyzebro.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2cwlewdmd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dkhjmtbf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nupthzdy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2fcvwtufw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2qcaxnfen.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2gyqnjhuz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2fkuzfuxr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2vczdaiiy.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sbkfbwwx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2jjboovta.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2dehhwgeb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2cbzudfdu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ilptrsxe.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iqcznhir.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2msyifhxa.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rvndretb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2pwgvlmbj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2hxogulzb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2pbshifaj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2qyziaedc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2pgckuoqp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2tcmcdvtp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2helygepr.html


<!-- 参考信息 -->