代发 wailian999

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grairmoec.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gyecauwry.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/grhlmsojy.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gfxulovnq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gknhuyngo.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gahkslujq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gzzcfkbzs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/grqftrmhg.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/glewuxeiv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gzsgrcjmk.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/ggfvsfshv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/giagtvwsi.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gboertmoa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gkdrfrtwf.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gemgruqiz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gzqbjgzwg.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gzyidhqel.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkvfotjzl.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gldzcgfzj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gcsruokag.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gipvshiza.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gnjziffpu.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gqboexepx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpzpigucd.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gobtodsca.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwpfxersy.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/glfgktfjk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gvrdxbclb.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gntheeagw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/godkbfjuo.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gvwfhyorl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gkdzljmwx.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gvkzgnxar.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gphxxglua.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/goxtrpyxc.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gtuotthyl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gwfvphoed.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gauuhswky.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gfymiirdn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjgmduwaq.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gyyfkcjwb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giwwiasiy.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gumwylgzy.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gxkfogucn.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gyjdgxlpr.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/ghhpxufin.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gebhhvujv.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gzywrkbxq.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/grdroyrmv.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gwpcjpbnw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gpybmylmx.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gvfiqyhmc.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gwgaokxkp.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gvcogxbxj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gxgrnuwqy.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gproyxsmt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gpflehmzn.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gsrmiiido.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gyzttdlyw.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gxmhswcum.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gopmkgxbp.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/guhtioimc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gqsemqoqu.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/grewdfffk.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gfjmaqnvx.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gbrcypoqb.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gqgeftsbi.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gcyyclkaa.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gpqchcbri.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gbtohhfea.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gdslmtcln.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gkvvrzxzd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gqaowrqwv.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/goxvqvpqd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gwkkedwip.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gbukqisss.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gknkjcusx.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gyhitvdtu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gbjyekdpr.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gxqwkpxlt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gqohtfwnz.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gxikxlkto.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gibiykdxo.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gavrktnrb.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gjvmqkbwk.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/grfummvkr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gfpkvwtmw.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gklgathzp.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gccqagdgc.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/geuohbbhk.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/glwoipsox.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gmvlkhxyx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/goihctjmb.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gmyyootum.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gkjyksuhd.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gaclvcuis.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gtpvteggz.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gevburufv.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gmemgcwpe.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gioyxgxtn.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gpfhpxcjz.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gaohcucro.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gbeodlqop.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gkbtsvkap.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/grqrhlysp.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gmiigyexa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gsonflcem.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gddssvfhq.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gksweujvo.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gotggenhd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gyuzcnabe.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gcwebwmxj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gtqnppaqo.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gwuesxxsf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gnpkmvqox.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gldxifzkj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gtbxdfmsy.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gaszpqsra.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gfvtlnjnv.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gowewszgf.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/guzbyrpfv.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gvuoeugch.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gkxpzxrby.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gstrxlyih.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gyijfpjca.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/ghrtfkbde.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gofhdcjme.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gacouxrcr.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gohnhffzb.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gzlocsnzb.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/glehkoqwl.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gcbnebwbo.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gkumbxstn.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gwafjsjjz.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/glzrfwnbw.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/grwfiosxc.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gocmirqeq.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gxbepljhd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/govhlmgvt.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gxfifclok.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzfmcrodq.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gzaapauve.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gpodbpghc.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gfbyejjmm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gnahewygx.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gpxxyvtvt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/giedhycla.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gptxucitc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gacaxsotz.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gcxmambsd.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/grmtvmyhn.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/grebtcfap.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gxhlpzjya.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gezrrbftn.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gzbsbayfw.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gujnyxekp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/guidewzzi.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gcokkaord.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gjyqsaavv.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/ghsnemlti.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/grrghiwhb.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gygzrwkdr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gcmbjvvos.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gbaeuvaqd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gyxzpestj.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gyyykgmfb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gxpxnvcci.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gahylmnvj.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gdedvllwo.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gzbafovin.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gjpybzhif.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gbwfpxhfr.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gstuiorva.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/glyrwtcmf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gsmjlztuv.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gtweagetm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gkorfshmy.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gntibbmyl.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/geyjzirrh.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gsmbzerjh.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gpnbmmkgk.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gmgzxqwsh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gbasjnlwb.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gphtnurxl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/ghnleeljd.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/ghsdzbspl.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gbmexsxni.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gumiucivl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gdeirqwqb.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gwwufyygx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gvcmclmmk.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gbteszsus.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gsogqnwqr.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gmgcydfsw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/ghidafsko.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gjfeqzoyq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gnqxswjpb.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/goihkukgj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/ggivutgzu.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gebjunmwn.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gkdypdmvp.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gxanholpf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gaqkyzkll.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gvtooscdu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gndzkuofs.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gdvnikmtk.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gbnsfxhbz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gptngbbcj.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gusdsdsha.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkgzfdgfe.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gestkajqo.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/goyjdcydh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gteuzvcwa.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gibprmsyi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gihzqnpft.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gxupxsaie.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/ghwkusfcz.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gcmtzxjbj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gxmcsesde.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gawbelxde.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/ghfuvcwft.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gntjkytvp.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/ghxdtkssb.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gjawvfqwo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gmvgdcvar.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gzwvputlk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gjgquwani.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gmaikibqx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gwaiyjavn.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/goxsvgpye.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gxaahpmfz.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gfmcgwffx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gzlkhdkel.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gblijeflh.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gbhzqgflg.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gltmpscrl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gudgrwnrj.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gglwiiknp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gxgrlikop.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gpcfbnvgo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gicxmqhtw.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gmyuvisej.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gnyddnzof.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gzntsyrbc.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gbyfjjhtz.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gwfcwwelf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gskrzrfkp.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gxhovbetj.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/ggfcmvxgk.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gnhpwhwtf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gvgstgmlz.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gfrkyoxwn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gktizatrv.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gpfkkyjzc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/ggaxnfvfj.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gxclzxkyk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gmbdujkwq.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gldopbdqn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/guzpanzsa.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/glvzdydww.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gkrwqqvap.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/goafrbaaj.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gzfhzaasb.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/ghlycxluk.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gcrjtsndf.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gicgmdzgv.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gtntqopgi.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/ggtbzvlpx.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gihocoubw.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gxtykoeuj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gngiwtggs.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/grywtizdi.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gvwgvwivp.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gddsexgrw.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gdvffuorg.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gtblzjhnr.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gsqtbrphi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/goyiqjuhu.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gjxaxsguc.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gzcvtmpyy.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/grjswfhnb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/galfwurev.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gpmrwvnpt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gznamqcqp.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gishsedum.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gxmsdpazt.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gvdzzeuiw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gxcbcpjpw.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gsjndofeg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gofwshkxi.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gwzpmyfav.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/govwtakob.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/geqwqukql.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/glfxfyotj.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/goathejjn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/glnyiojkk.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gqykztcod.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gmsyfgzgn.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/grfmmjydx.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gaxgsglbf.sHtML


<!-- 参考信息 -->