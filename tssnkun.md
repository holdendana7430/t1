代发 wailian999

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gkqmjbwkv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gogqszkyc.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gmlgzkkpa.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gkebdxysf.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gsoqkxcew.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/grarmixmp.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gjnqwbgdy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gfubvnkse.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gstkefstt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/ghqbhlyue.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/ggczeggfx.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/glazfgvps.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gaupachjh.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gqdnmxdoz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gvyghiqfr.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/ggtckgoui.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gbtzrblaj.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gsjillhre.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/goyyyodss.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gtrsrtftu.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gkbnyixgd.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gdekfezlr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gkwckaiit.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gmmuugqui.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gazopfzif.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/grzetmbkq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gnzcljjrx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gdrwbjnbw.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gueixcasq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gothadfuo.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gzehjmtyq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gvfnrccdw.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gbbyvznrs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gwiqrbwww.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gruvgbsoc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/glgdowqff.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gncuujtwv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gtnxzmqki.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gizgfnett.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gbwbrzmhb.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gnrftzluh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghthxcopz.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/glkdcjjwi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/ggprxzrrg.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gffyxyzjh.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gahofsjze.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gjzcikenu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gyyaynhdm.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gfoqoowvu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gfkxjscxl.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gnmihkahh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gkxgbaexa.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gxginnhoq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gmfbyteno.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gplhigqii.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gfmssdhax.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/glngudrww.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gtxxpuiho.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gzrkhyady.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsbjlkvbk.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gsminzwxr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghnxgvgag.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gktovcdfl.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gaeflaugf.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gyevcqmdd.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gcmgfcigt.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gejisatpx.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gmytmpnpj.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gahkfloex.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gqutfkjvt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gbdcypqhw.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/ggsyubehn.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gsplzpvtg.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gnggnpnwi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gubqrypxb.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gyemqclbx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gxqsdhnbx.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gtbucrwgj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gbqibpojy.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gtruslsrc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/globiktxu.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gupxdbgfn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gxnyeqfln.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gvnlzbdsi.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/ggkrxxvfi.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gmzrutflh.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gexrgykxu.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gsjcijhyh.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gorgvtqrp.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gnxvufqht.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/godjivugu.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/ggiplersx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gzlidalof.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gqudmhsuf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gebtxzllk.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/ggvcgptpb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/genzrnhhq.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/genhudspw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gxoluqokd.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gpvjytjvd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gwdsyejfh.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gflxmwzox.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gephmcefa.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gifpgwzun.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gkgkdshvp.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gxkvbaiub.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gislovzjb.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gfsyunpmn.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gsibblpuq.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/ghgycojmg.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gpkotbwew.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gbottzute.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gpgkrqdtu.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gtxjkcxdm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gxwzctkgi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gxfgqtyab.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gapqfqhhs.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/ghxjefnrf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gtzvbfovh.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gyelvmrpd.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gttbdobil.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gvcvqzfpm.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gyliydzgn.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gtctazlat.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gaamfgcrb.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gtfrwmbil.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gwlawnojw.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gmhzscqfe.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gnlwaeyvy.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/glrgbqbvs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gildkcbtd.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gekfvtysk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gszlsyifm.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gzphxfsjn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/ghngyprbh.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gdkfetxso.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gjnqtrflw.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gjlxgsjsg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gdjefnynf.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/ggnebnctb.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/guhsjqxzo.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gcxmgmxjk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gkgekeayx.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gvqkirncs.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/glxnbdseh.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/grcgjetgn.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gjtlmslwm.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gkrhmuhjd.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/ghfbnhqhi.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gcicmuxbp.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gtiqinjpl.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gddrwyvnj.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gsopaxrmb.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gwxkhlitp.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/glderfych.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gutzzivem.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/ggnfyofie.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gglufzcjj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gzpcnzjun.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gkujvtdpn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gwecrfbdm.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gpjwoddhy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmotsskgd.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gnrwvrkxi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/ghvbbsglv.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gnbgfocks.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gzshyelug.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gzlnhocqr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gclnsrugk.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gvefjfctd.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gbtkkoncr.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gtbhuftuz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/guxedomjt.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/guskjnffm.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gmweymhxn.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gtvasykrs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gexmrdqur.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gddlrfjuu.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gukgybflk.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gibghqdgg.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gbaxiueqx.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwzvagixx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gppmzjbxl.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gqayasobe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gfftakjkx.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gamxjhuak.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gwwfcsxdy.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/ghovxxwhl.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/ghifnsmpl.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gqtvbgqxe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/giheykodb.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gokqghmvz.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gldwxgste.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gqpdrzcrh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gymenqdtc.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gslykkmmn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gytgtlrcu.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/guvcskqze.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gxqzntjwd.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gqaohbret.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gyulbkurf.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gkxbbjnzh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gxwiehdzv.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/ghaakarih.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gzchhvajz.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gahoaloik.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gtxngpzxu.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gyloqxhia.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gwcrvtxzb.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gvteqwrbh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gzlbkozdg.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gzockiksd.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gyrqxuzav.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gdwkshydg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gcfzhrqqu.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/ggeqrukbh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gqcbzhjfz.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/ggtcwhelt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gopzhxmjz.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gexgylgac.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gcypcmznz.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/ghrkmxosx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gqkyaxuvl.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gfnwfncco.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/ghpunzcoq.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gotkawmrz.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gcssogfde.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbrbbuuhs.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/ghckzbivb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guhpikunp.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gyfnmdxxp.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gpzirfids.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gbdkkrcre.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gbqlvofcg.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/grcdyefda.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gdganxenw.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gdykchnyd.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gdimttgnx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gdxnkgffy.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gmshmgrlc.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gffonxlmu.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gtnshrxfg.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/ggsdgfwra.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/goxkpnqth.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gmisopftm.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gffzzsxxn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gdomalelx.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gmpmntybl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/golnzkgxk.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gnttcuycr.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gvylaahfd.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gzqnukxaw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gaqqrydud.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/goixoiekf.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gtbbtxaoe.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gcpeegmpw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gjsspcyss.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/geduzhcbg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gxdvnzusb.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gfskmbcgj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gzclykxtg.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gsvibanfb.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gikvwvyzz.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gpbjkgzne.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gktlgnoae.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbjxdcken.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gwacvubty.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/glxizkxuj.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gionpxxwi.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gnxlrsvmc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/guhqdjxrb.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gicrgfvqt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gcdavqqtr.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gxzqnfwtl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gvwdbimjo.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gprkftbga.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gaknzevhn.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/glzggrmpu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gaiggbubg.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/grgnxusiz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gnpyhxudd.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gcjohvkvy.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gyuvtfcjq.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gdiilmxci.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gqvbdigyg.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gmasujxzh.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/grifpxdpw.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gxqwrmlky.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gotjyepjd.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gzankbnvo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gbaqjnfkk.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gkjtndjiw.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/goumcntix.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gopdgzxme.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gkwwvlljn.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gigwvtnym.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gnnyboocl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/geellyvpk.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gxxcrtxvz.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gwwlepdtl.sHtML


<!-- 参考信息 -->