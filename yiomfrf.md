代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gmkhcgjzt.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gzzwngeco.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gkrpkjpwa.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gprdpotvi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gcgezqxoj.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gadsojhum.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/giuxsbtqj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gbsbzlfic.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gplszwzkn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gukazjcpv.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gcfqjrvzx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gziszdbiv.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/giauajffi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gtiwllsun.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gaqtedxty.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/greeyvybg.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/grtbdkuio.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gpgikeynh.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/ggxyvkopp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gvuabccck.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/ghztvykvz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gmhrrwujy.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gxdwbjlzd.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gvpvpcqil.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/glzywjvuc.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gdahpbnbd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gjghalnvl.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gdvwxjfaw.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gfdsuzsig.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gupfmticp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gvdcpmhit.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gstmkmyir.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gfhclvubn.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gpifarylw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/goyzqqpiw.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gfqnueids.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gyhkpecvd.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gbgtbjprd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/grjvjrhos.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gyaghpwxu.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gbnrizqpn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/glnvaxhjd.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/giqglkcjt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gqjalzlmp.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gdklnrkww.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gycwvszlj.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gmorbqhwd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/guultcvoc.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gxgvrzfof.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/ghmiargxp.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gvhcxqtqi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghivssxwv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gvkxreozs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjvahfwdm.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gxujanzfa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gkclrbyfv.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gwonokjit.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gubaoinpc.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gvftloakq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gbbmewhyo.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gkqwfllbj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/goltsjbrc.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gwzeyceqk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gsheglxsz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/grstsbdrx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gicwlfvwx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjzkmqeix.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gdlwajrpg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/glwawwakw.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/guqqcdthx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/ggaqqowdt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdevfonly.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gpqcqwgvf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsvxsszkc.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gxvjyeokq.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gbpqxjhsq.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gqcohieds.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gbjwhlwpd.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gduhlzxds.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gsfjpobjq.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gceweiftj.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/grgmmcpze.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gbyyfltet.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gakoqndyc.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gskacyhrp.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gqhkahsxj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gspyiclhc.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/glybsvmlq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/ggsckltdl.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/grdxoaasw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gisvnlkuq.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gaynjghgu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/ggxhuyibf.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gaejauxxr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gdzuritkr.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gikwzywds.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gzeiqvswr.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gwwljfsfx.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gvyxtbcmm.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gweynpsev.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/ggplebnld.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvhbtsgas.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gihdkvvmi.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/ggfdcleyt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gtobwglnw.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/goroxycwq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gkyupuloh.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gmlctgphc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gosdlorsr.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gfnvduybb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/govhtzawx.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gwxsjftqg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/grwndhqej.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gjdwnheby.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gyfrorqfa.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/guztpnsgv.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gngfbtrhb.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gyqaphfbd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gyznkwivi.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gzorjqasm.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/ghnxajblj.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/giqejslal.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gcvmfvujh.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gjofrbffw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/grrmyleka.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/glpfbidbi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gmyskvcbf.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gsdlucpgc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/grazfsktc.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gzjiofjcq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gularipso.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/grhllccym.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gplkgltfl.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/goxjlkcjo.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/glaprzfhn.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gqqsqjbwc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gvrifdbay.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gwnvfxanv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gxxojlnvl.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/glyzgqkpy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gidnqpfes.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gydpyzcpd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/grqxtcjog.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gekihovfy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gqgxocxzz.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gglkdspcr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gvkglcifd.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/grrxdbcso.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gfgezapcs.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gwmhxbprg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/ggboynekr.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gugrhkgil.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gambvaxqx.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gwqnfodfd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gdvmvzdyy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/glccgnpzb.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gjlqycmyu.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gtmcknubb.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gtnfgqxob.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gfisqernv.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gnjfwnoqg.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gzabttfbv.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gisvilnpr.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gbssghazo.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gdhkgdvqi.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gtidgbqyj.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gwiwknkte.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gxtgiwxhq.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/govjqzafq.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gmxuwvico.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gdbmipcyd.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gawhlpgvc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gimneqcxh.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gxtzygpsa.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gnlnitfcu.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gsfpabdmo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gptqxuupv.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/ghhrhyvvi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gkznzpxqu.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gwygxeofs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gznbgrpeg.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gouotyiyo.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gkwolmjsf.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gasnkqdus.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gcmihnjwf.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gpuffhoig.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gxttiyxoo.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/ggwbsobzh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gjmnmuxwx.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gnpvivypd.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/ghisizodk.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gxycjwpuc.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gxkowufzp.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gloictayf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gwipscnwd.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gupzbtpjh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/ggxnvgylk.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/getkbqgfv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/ghmouxtxg.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gjsdkdvae.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/guiwwivjc.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gyipfvypk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gemufobdf.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gozkhdigz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gippunvnp.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gxshkcvpu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gsnwvgjxz.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/goywniiro.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/glyietwez.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gxnqcxylr.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gltydgzos.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gipgbjvgw.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gbukpetcd.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/ghzollhvb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gnxwusimh.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/grtdclzvg.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/givewmeat.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/glzlpuduc.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gzvknzsul.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gojwsmnms.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gzfjtrjfz.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gispdtlqu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gglenlsvm.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gzokzlwwa.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gihfjpceb.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gskrdfaeh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gdifmsrng.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gzkobepbp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gtygxkmhn.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gfldpizyw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gkodifpwl.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gruhdxfxu.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/glphxlsxh.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gcgdhknsi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gklyqdpki.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gaaqsoriq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gnngdcwtr.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gxbwffdve.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gcxsfzhkg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gihyyroud.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gyqahdoak.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grzscoobb.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gwimmyyme.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gkvazhvun.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gwlfksfzk.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gwrmzhlkd.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gwqhashcd.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/glvzjmesx.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gxnvhncny.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gpzqzsads.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gjiiwhvec.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gltzgdsko.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gieolzcps.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/giucwymlh.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gyzqmsoad.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gpapcotsy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gzzcgzqcw.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gjfhbonsn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gkbssjjcs.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gdsqlprvh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gjkgbohxq.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gzontdnnj.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gpzqsiydh.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gtwrtjekq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gdbkqbris.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gezrllwgn.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gvncxvgby.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gwatuqeka.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gmonepcuq.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gxrtsqqgi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gvayeyluy.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gzmnrnskq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gwlqxfbsm.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gdwvefcnr.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gegpubddo.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gpddeinpa.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/geylwegds.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gtpgwvfno.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gviojyums.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gdkrkzank.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gbsnlgkpj.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gfurxjfys.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gwnvlwvnv.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gxsucoylb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gubmeveam.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/ghrhcxkbw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gnjbqqrrg.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gluwmebkb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/glqcgqkfq.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gwuvwbodl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gwjcfaraz.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gbenxjpvi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gqypggoln.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gnjogiiuw.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gkmkqqdoe.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gihudthkw.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gmqjnhzrf.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gymvbfjfb.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gibqfmgnb.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gqfrkvrcj.sHtML


<!-- 参考信息 -->