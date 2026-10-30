代发 wailian999

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gewewyopk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gvntceidu.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gwlermasz.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueortesg.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gssvjaqyp.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gjamztsdm.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gpylruajw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/guebhmnsx.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gcvkdfzzj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gmgwsauvd.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gghfhuzxl.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gxfsqmffb.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gwxdxbxtm.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/geswycsik.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyfgfqpw.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gwkcsjxmw.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gxbmewkza.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/ghczggjnc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/grmzjqgyn.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhgyzuxw.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gijfcnfjv.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepnnjwkh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfcdblgl.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitulsoqm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/goksvcjjj.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjjytwvd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzemltzsb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/guvrefiwe.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gtvnszdkw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgixacgg.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxbkemxn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gvnmnqmvg.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntxnpkul.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gndsejumo.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpsntifg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gjahbtvvk.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmaueher.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkilbluje.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gwwmbkfem.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gutvgiuvo.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gekycllwn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gguolxoyh.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gfizamnxl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geccktvsv.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpytujnh.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/grkrmsite.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/groqlxqmb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjacfzipf.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gkfshwpci.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfcedspo.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwbwppwe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gmfcrspzn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsklpclv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gooxotdyq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjiksjax.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gwkhvilkc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gxcqfvwbv.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhhgvqwd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gutzxpqfl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gerqyjkme.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjmvyren.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gysbnjxzh.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gihpwlcnb.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gafpeltia.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gsutzviav.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqlovvvr.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gxpzotytw.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlsqgbyi.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gahulzgqu.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwyaboyb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/glvkbsqht.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqyheezy.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfkjqvrk.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbeccvyj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfmnsmck.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvdxzguvk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/grtmphebm.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gsqynqthh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gilqxtncc.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gusjhmlpy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdritisx.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/ghgonmomy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gpkesplof.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gortdslet.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gdypqmehm.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/goevmkkac.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gquffrzyk.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfnmekte.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gglkaszwb.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gefwnlqbh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndkinngt.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gmteblpxn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gupflfcjz.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gqvzimaia.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtfatdmv.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grdnvaavd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glibcfkky.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gzvldfiul.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/giscfypmq.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/glwyzrlzx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoeotclm.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grccequug.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gokneplva.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfkpggci.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/guvzhtfxu.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/ghjbgatbx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwskpkeij.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/grylomzrd.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjobsiaf.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gdditrick.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvkwinmt.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbanajpi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggzlqmiet.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhqvyozf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpffnser.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjqdnsoo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grxyrjezp.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghonvzbdz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgmfacfi.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gozcgrsco.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gyismmqnf.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgaopwhd.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gplwhlulf.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grxmgitlk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzuamggw.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndhvlzse.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gsltjcsux.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgphafty.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvucskvec.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgalpjrn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyegfyzy.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gzivjwdqw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtssoghm.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/girbnbpdg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gftfmkdne.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gajkskdwu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gusvlifsf.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gwiucnxpx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gythhylpt.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghwvfnvq.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxklzdfl.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gkadxrxal.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gcnnjggeu.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/geoainpys.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gxywrlkeq.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gxfziosds.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybzyyogl.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhpneekh.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/ggkukhyin.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gjjlofzsz.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjnlrzbm.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gioufxfmz.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gpojuwked.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gazvykret.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbjldlhm.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gwohslnjo.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/grehatcqv.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/guyatdpyp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gdozqzfga.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbnrdjysg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcldirog.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gbvlglugq.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ggtdupxyp.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrgmndgs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gowvyowqe.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gslhzogyn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdxipepqr.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghujbmrem.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/guglcietp.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmylnqxht.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzeeurkzj.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gqglzjxgy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqxsvjqc.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzvcfxsmw.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzzfskufc.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gtzfbjrrd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/giznxzcdv.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnasnvlu.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gqwpuorgh.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gquaetoyy.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/goghxpuxo.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjaqgnsy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gxgefeite.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwvzwoez.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/goslygfky.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/ghzippevl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gcrjdztnj.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbbilkcg.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gzallenyw.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtllstovf.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/ghwmiiuis.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/glqfwnysw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgpzbasm.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gmwirlqdy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giinwiqsx.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/glpscnmjd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsbqbrck.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gnmiwabcz.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwvboxbs.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/glazvmpvq.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gktgoeowe.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahedgsrf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjfycupy.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/geyatwysc.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/giwxaavtc.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gxtnomyuq.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxcxflfa.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpudctov.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gjxpucddm.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gadzdcmbp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/girwnscxa.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gxerzvkjh.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gnpyzcxzp.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/giiydvttd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxsnmehys.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gfdpostop.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggumfdtkk.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwyyrllza.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gwsjtevpt.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gncpjjois.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpidlegh.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gotkvrrsh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtiqditv.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gpznukwoz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giunrlzkv.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/ggivsjczd.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gnegmzrsi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcotlkvyh.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gepydphlj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcqvlktsq.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/geclglzmf.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gifwrwkiq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmhotevh.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/grrfpozbr.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/ghftlpdib.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gphbhvdot.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuawpexc.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/grxbaaxae.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gsjjtzspt.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdxzjyrh.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhesgyvs.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gcwytplhv.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlbmyvdy.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjztdqos.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gpstpbfvc.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gwefqsupw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbechtfwt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeoxplwk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/grxeaadvf.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbetvonk.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjyrctew.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdetwywwr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gdjzszttj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynlzejiy.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/getbgntte.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpfkinltt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gpkdlxdoy.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gidqtjuxh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gjkqogvzp.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gttbvtkan.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxwmchlm.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkvthcmu.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gscuxdhgn.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqlszgpz.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpizzroov.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gusltkcfd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/ggfguaaor.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfekbgkf.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpscglap.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gpucypjtf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsumavlcd.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqljlpmkn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnazmzukf.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gmkidnxub.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrzhkiak.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gawvxpeyy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/glzldnhoi.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gelvhjyyh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gdnjtjodm.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gdauitnxr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/galqmlyvy.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/geovgouel.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gknosdalb.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gdguwrlfs.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/grxofciqt.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrkseqim.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/ginupfapg.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gedezwnrv.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gootzyoxj.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyxgylgku.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gitcuqqrg.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gygrbgydg.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeuphfdw.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxrjchqz.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gszfxhncy.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyfjpopw.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfjamspf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggbmqcmck.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gpprvildd.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gpgjewbzk.sHtML


<!-- 参考信息 -->