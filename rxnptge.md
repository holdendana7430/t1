代发 wailian999

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gdfgfkomx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/grhpqfpql.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/ghojpqeqn.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktrprovh.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrrqkwch.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnmzidhy.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/grwylbqvo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/grijiwuci.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsuvccgh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbxgspuc.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhbetvbc.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafnkkutb.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gymwddijr.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneyapemy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/guqkbthmv.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsanvkufx.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldoabpux.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpzfviec.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gfwcqjhcs.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/guuxipteu.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxesjdjj.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpasmpjs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gndbubtgi.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gszyrwnsw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuwyykav.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gjyjqeojq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyarewnl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgzicjni.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/goolxlsov.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gskpmwvvu.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gosivcrel.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gbmzfmgaa.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvvdqnka.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhnbvjvo.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gristdevl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gxhlrdzji.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/glhmuapwk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxekbnvz.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gfvhblaok.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grmttrifx.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gprqzjkcu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gyjrbkhgc.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gzcpwueuv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjukrveap.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjqbwtuh.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gajtnwbqz.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsrfblrq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/ggdtemecd.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gyjkkpdcl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbmimgsd.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvsxssnj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxejmwhxi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyudvmodm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gloewruip.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfwstjjnk.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyopwqdoj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlmhdznf.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gsztqerfo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvznenywa.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqsomfkp.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecrzsxco.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzasvljk.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouzqkfff.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gqxyfuocs.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiakwduz.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqdeqesm.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoqrwpwh.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gosrdacao.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqitxqltk.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guklzctho.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkvlyrob.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gigodleas.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrgbqjzf.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gksdlcvkn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbvwshoqh.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guhivcybt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gglzhuktc.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gytypriwq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/ghwabqkzv.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfkcsynk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/guyerqhuq.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gnceovect.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeqngzer.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gqcvmndss.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gbrvolhcb.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gwebrskvl.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrysozpg.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gklzzvrhv.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gfvalryem.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxmntsdxj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnowpywmm.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaaxapla.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gewwbzoei.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gojqgvcue.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/godwggyse.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnobfmvhf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/geqlbndoj.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzgztbgq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gifqpoiqi.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaagzbup.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghfezweff.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gcawzxddq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmxddmjia.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gglucqbjz.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjbrcogne.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvktruhzb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykuksrgl.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrtxkbne.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gsrguhbmy.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gmtpepjkv.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvbjbiitp.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gxrggbmfx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghblcqylz.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gabjgbxhs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzrnphzr.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gkvtqejzq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxvtnfuwz.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/groouhitn.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzrfwrih.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqofjovtz.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gimmnbugw.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gfowwuftb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlhrapim.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grpkyghvj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gqslsnnjq.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/ghtqvdhil.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxbitxpw.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuxhrsgg.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyquwdsiw.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtasdwyo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtctsqdca.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gppmqkovp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/grxtbtqpe.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gnujjfysy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxbwbxpw.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gvprfyytk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghplopukv.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gssdbwqiq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gbikcracm.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gcyxliaej.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gacmlxsgd.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gecghhiai.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gwubimliv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggecjwarq.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gobzeceum.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbtzozzo.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvogrorwa.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gvndbekkd.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrplvdcu.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gorvfxgwu.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gamhvgoza.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoljlqwn.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/glhihdodh.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/giwlxbghn.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gjrhkqmvh.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gsxhjfnpy.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvthkexj.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/geqrwbidk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gekpyfmms.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjvvxwor.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gibbqrxwm.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gxyrgjils.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gajxqhigh.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganzdtzzl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gfskkqvqk.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqaxvcdw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpvlkqvd.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gtexaigos.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyqmouiz.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvnnzjbm.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxnikkqz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkhdpfgz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/goizejuip.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gufmkovxo.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfngnnuik.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclnpjceu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gfqbwzdix.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/geptznxpm.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gfthgzykk.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/goyowwezi.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfxywbmi.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/goavydreb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwtosodz.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gboiuxeka.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/guligehss.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqzojlzn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvwtgurs.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gitsjdoqi.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnxxwybz.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gickegeyo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gslzsgzls.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzctdicxl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gsutsbtiu.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmbxighy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtyengcj.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glembulvh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gihpdxpub.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gsszhssoh.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmxqssca.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/ggspsmkhn.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmgnpboa.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtwlltjh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwpjmerx.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzajzzvg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqtydjjy.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gslmeqajc.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gzorgfhni.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdeiigwv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/goxnlqaal.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/ghkgzasai.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkhegxdis.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsziqukg.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwvpkmlu.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gevuseurj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpnewwvsg.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjchwfqt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gspvskqiv.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvecyvgum.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvjwdach.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gkusjyfqa.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsjlkrnz.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhvkgwih.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/goccthbeq.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gesakevhf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfdbenaih.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gbubtbuwg.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/glxrpyrep.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpntjmqt.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ghcfkrbgv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guwgwnbyo.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzxxftmz.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gliswowip.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnltkadrw.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkumsjam.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gxsdsnewm.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gljpjvibj.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/geemwvzbt.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcuzhprq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gflkrjccr.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvxuigbi.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gdctqfjoz.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgqvskgv.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/geokdqhnn.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpftnbpu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gbljtxnyp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmzwjgde.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglauiapn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gswuwqwfc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvmzvyjn.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gnkxwbdye.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gmfdnxjkf.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/getsrkfam.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/grcnlurqg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gadyrnboj.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gddvnxzrl.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjlfdwdjy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gillgwpbl.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gmpolvutb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyupglpo.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gvnlgrkbh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gboeukhat.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gloxhwnbe.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptpvotyy.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzwxdvch.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/grwgffdjv.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlfsqrkx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gjrcjzhiq.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpyuuqvd.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/giziqhqlz.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gxqlrrins.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gkpqkwmae.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkcdgfoe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gunqumrff.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonsfthhp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gwwjuwham.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gcstacfta.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gepcwlnpe.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gnxtlawcf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gyvcieuzd.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwlsfmvi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxscjjzw.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gyintnoie.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gubqtercm.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfaoqzyq.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbxkxxsp.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkanfrkgf.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbpczqgw.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpurxkugy.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/ggcjodcml.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdppavpth.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gialjcdvs.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gqebjyqsj.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqyjtzxm.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/ghhwrjntj.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnpmnjfm.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glxzbxmam.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gvkvwojjw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtxijatvd.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gwaswtffd.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvhoship.sHtML


<!-- 参考信息 -->