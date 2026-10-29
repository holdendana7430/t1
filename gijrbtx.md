代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gqzsfzcek.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gwxeunduw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/ggnigpkyc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gqldtzyjt.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gwmplkhdh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gnyotllln.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gvwnilkkk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/ggrolxozk.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gvseebylv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gofdhiser.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gnfitdgwo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/ghhjcixfu.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gcrzsvhsa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjsypejvq.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gibgpifps.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/ggjjgagnp.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gcdshysfg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxzoazrnh.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gxojbccsw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gujyfznvm.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gtahgvrsq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gaoivkezt.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gcahuadvf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gwosyocro.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gskoeylob.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gkssmmgmc.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gwsydckco.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gyknggpmd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gfwhdjvah.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gphindamk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzghrowce.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/ggoslnpkn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gyhzibyev.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/ggktypevo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gxwtqehwf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjealpakk.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gdhdbpbod.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwnpzkmce.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gfodjwpjf.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gtgwzhodx.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/grahyoueq.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gwbbzxscm.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gbgqmlyof.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gwwgrrfxp.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gwgwzqkcj.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/ginrsdleu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gtupudbkg.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gixollgny.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gfyrpurbz.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gyurqvmln.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gablsvcrn.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gopfevyyj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gpwppuwks.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmhbcrfab.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gnaqgripd.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gpynhkbnw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gpmaaxdnb.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gqohvolwy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/ggjmiubzg.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gkwujpwpx.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gvvxjxuem.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/glvneymwk.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gmakfbgfu.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/glarvmlfs.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gkiymmfly.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gpvlqutft.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/guajnlooq.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/grfdujzad.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gduqhrxly.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gozjblcpq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gheadcvwg.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/ggemilkrl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/ggidposvt.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gfgmrwiei.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gbztojklz.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gpcalkggc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gksguxjdk.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gomngybrj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gnxouafmk.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gyjukakai.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gtzinwmtw.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/ggxecnpiw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gbxwnlpqv.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gmeybvmqg.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gzandijxz.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gbeqqfdpr.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gdzcndfpu.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gdstvduhz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gyxtlsdpp.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/griybdezu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gkbjamgby.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gduluesgf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gdxppdzxo.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gugsadeko.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gmmdjopug.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gtbtovxdg.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gocdkqcby.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gecmzhrba.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/guovvaeyp.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gdmqpcttr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gtadbkoax.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/glkutsbph.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gotmrinrs.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/grqhmuuhq.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gaiponkjb.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gveyjwjoz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gbmhpinim.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gjnscsymo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/glgjwhjnt.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/glkzsdlhd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/guiqcsvhs.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gprbctcgi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gjwpowkut.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gvxbfyosu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gqbnhepnn.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gueeuwnvv.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gxgkksenm.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gufeazmop.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gitnahshs.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gsdykjyqt.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gsiumxqxg.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gjwpnaqnc.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gwhwtykeq.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gabofhxyg.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gzbzpmdui.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gzmfegzfa.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gdxivqtkm.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gazjsaqcu.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gdllxjsld.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gknvzehwy.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gxaggiehd.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/ghptyygsd.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gmlhcauol.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gckuoakdl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gcegbzuix.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gljbjftnv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gpnvnfyvb.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gfdjcuxgv.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/ggwsgxvjs.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gzhqstjse.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gahctpbzp.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gcvtsxsdk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gdzklsaak.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gtwusscgo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gnhibtvww.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gkxshfizx.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gaqdrvzdv.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/glqbapycq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gabmrrvgp.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gbeeaaeku.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/ggygwaiwh.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gptfijtar.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gmgzmgvjf.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gckmukoqf.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gwhhuancz.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gtekvgxvd.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gkqxakucd.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gcturbvzr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gpukigshn.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gjgpenbyn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/goavocvmb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gqbvydxzv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gqlsdiwtg.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gntqjegtz.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/giihduxof.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gqjcofmgb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/giywgieee.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gzqkevuyi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gticmqvur.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gapdkydlo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gpkiofvrg.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gtiyadeax.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/glnlcojab.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gbpdhquiv.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/ghpoieupu.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gbrxehuen.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gdnvaareg.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/ghaxfmqox.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/ggetjodsm.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gtbbllpwa.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gtiqeqouj.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/ghcnjgtuz.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gcxgaiynr.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gwgmykwju.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gfcsxvpyr.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gqzutbpri.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gyotofgxl.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gwfeilych.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gkbtzygzx.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/glnpcmuhs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gytxnehps.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/glpdgfgdo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gkctadukp.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gvmoyxxbl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gyqlgjwjo.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gfqsehtif.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gsepzxnmm.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gtmnycnxa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/guuxlpowp.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/ggdifgesh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gmiiwjmuo.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gszutweao.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gjfdmckrj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/graiwrfxn.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gvnwxfiis.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxplulkvw.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gdbclqknx.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/ggdxdaioq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gvumbcajs.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gkrnpotnk.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gmvukavqr.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/ggdobuvdp.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gkyxcnktf.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gvmioditk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gjryupzze.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gdviiewor.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gzivbuqvo.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gtvrpxyov.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gwtklpzrf.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gkggorman.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gndvgissw.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gucjbfjsl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gtidpuvlj.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gjwahailc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/grihxcyjf.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gffwihdzk.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gjycylnyf.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gwtrvokiu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gejjwmzjl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gtonpdswf.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gzcbttdbv.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/geymkdapt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gnqekvjmb.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/guifmvwvx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gsjgxrwwp.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gsxbadxak.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gozomvdht.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gxdaxglod.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gupwvthyw.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gdzfpocrw.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gniqilaay.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gkbivcghr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/givexkrzf.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/geebezsql.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gnijmcspj.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gmdfcqqtu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gjdpjwnok.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gnofcywua.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gehqjtmow.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gyoiodhnm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gzfjxwqmr.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gvcqqgetf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gzbcbpkbf.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gfnfpukgh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gnqdliyqe.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gtthcnkjs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gegicfufa.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gqckjgxsq.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gclfkrsnc.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gowlcnxgk.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gvdqzxdex.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gnxpinerh.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gwbhejcib.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gcvfokkrz.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gslzojzlb.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gppaikyqj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gntpjlnwl.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gufvnwkdl.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gzwyukyjz.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gsrsrpfah.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/glqhxkkut.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gtcbvdynp.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gxeikvqoy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/ggaxpjwob.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gyabusbaz.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gwdrvxuus.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gpwevmynm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gtjpgkkrl.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gvchpwbba.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gtqgimqrw.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gkeokbipn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/grhoumvxf.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gtvsyuchu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/goujvjxmr.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/glrnyirqz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gglvlgrve.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gxkhcakkw.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gnmzarasc.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gwpnmavxe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gthgwrgyz.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gfibxxzja.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gnvzyayzf.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gpqjrvqea.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gaidwcffo.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gvbmngnzt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gwfwfoplw.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gxjvzeiuy.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gsfopxwop.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gdddcdfjh.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gtctbuink.sHtML


<!-- 参考信息 -->